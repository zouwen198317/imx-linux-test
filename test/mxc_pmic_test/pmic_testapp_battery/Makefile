#
# Here are a list of OBJS needed
#
TARGET=pmic_testapp_battery.out
SRCS=$(wildcard *.c)
OBJS=$(patsubst %.c,%.o,$(SRCS))

all : $(TARGET)
	mkdir -p $(OBJDIR)
	cp -f $(TARGET) $(OBJDIR)

$(TARGET): $(OBJS)
	$(CC) $(OBJS) $(LOADLIBES) -o $@

$(OBJS2) : $(SRCS)

.PHONY: clean
clean:
	rm -f $(TARGET) $(OBJS)
#
# include the Rules
#
include ../../make.rules



