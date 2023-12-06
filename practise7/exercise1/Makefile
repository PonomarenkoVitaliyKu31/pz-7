# Компілятор і параметри компіляції
CC = gcc
CFLAGS = -Wall

# Директорії та файли
SRC_DIR = .
OBJ_DIR = obj
BIN_DIR = bin

# Вихідні файли
PROGRAM_PARENT = program_parent
PROGRAM_CHILD = program_child

# Вихідні шляхи
TARGET_PARENT = $(BIN_DIR)/$(PROGRAM_PARENT)
TARGET_CHILD = $(BIN_DIR)/$(PROGRAM_CHILD)

# Збірка основних програм
all: $(TARGET_PARENT) $(TARGET_CHILD)

# Компіляція програми батька
$(TARGET_PARENT): $(SRC_DIR)/program_parent.c
	$(CC) $(CFLAGS) -o $(TARGET_PARENT) $(SRC_DIR)/program_parent.c -lrt

# Компіляція програми дитини
$(TARGET_CHILD): $(SRC_DIR)/program_child.c
	$(CC) $(CFLAGS) -o $(TARGET_CHILD) $(SRC_DIR)/program_child.c -lrt

# Очищення вихідних і тимчасових файлів
clean:
	rm -f $(TARGET_PARENT) $(TARGET_CHILD)
