TARGET := helloworld.bin				# Name of program
SRCS := main.cpp						# List of source files
OBJS := $(subst .cpp,.o,$(SRCS))		# Replace .cpp to .o (subst is a make function)


#CC := gcc 								# The c compiler to use
CXX := g++								# The c++ compiler to use
RM := rm -f								# Linux os command to remove file
#CFLAGS += -Wall -Werror -Wextra		# Compilation flag for c source files
#CFLAGS += -Weffc++ -Wsign-conversion	# Compilation flag for c source files
CXXFLAGS += -Wall -Werror -Wextra		# Compilation flags for c++ source files
CXXFLAGS += -Weffc++ -Wsign-conversion	# Compilation flags for c++ source files
CXXFLAGS += -std=c++11					# Compilation flags for c++ source files
#CPPFLAGS +=								# Flags for the c-preprocessor (typically include file paths and symbols defined on the command line), used by c and c++
#LD :=									# Linker to use
#LDFLAGS :=								# Linker flags
#LDLIB :=								# Libraries to link

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CXX) $(CXXFLAGS) -o $(TARGET) $(OBJS) # One single tab must be placed in the beginning of the line

clean:
	$(RM) $(OBJS)							# One single tab must be placed in the beginning of the line

distclean: clean
	$(RM) $(TARGET)							# One single tab must be placed in the beginning of the line

#VARIABLE = value		Normal setting of a variable - values within it are recursively expanded when the variable is used, not when it's declared
#VARIABLE := value		Setting of a variable with simple expansion of the values inside - values within it are expanded at declaration time.
#VARIABLE ?= value		Setting of a variable only if it doesn't have a value
#VARIABLE += value		Appending the supplied value to the existing value (or setting to that value if the variable didn't exist)
