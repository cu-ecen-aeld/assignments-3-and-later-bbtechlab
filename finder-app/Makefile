CROSS_COMPILE?=aarch64-none-linux-gnu-
# CROSS_COMPILE?=
CC=$(CROSS_COMPILE)gcc
SOURCES=writer.c
TARGETS=writer
CFLAGS ?= -Wall 
LDFLAGS ?= -pthread

#rule
all: $(TARGETS) execution

$(TARGETS): $(SOURCES)
	$(CC) $(CFLAGS) -o $@ $< $(LDFLAGS)

clean:
	@rm -rf $(TARGETS)
	@echo "Clean $(TARGETS)"

execution:
	echo $(TARGETS)
	#chmod a+x $(TARGETS)
