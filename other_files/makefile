####################################################################
# Makefile for building the clinicQueue application
#
# Definitions
#
CC = gcc
CFLAGS = -g -Wall
CCLINK = $(CC)
OBJS = main.o clinic.o doctor.o patient.o
RM = rm -f
TARGET = clinicQueue


#
# Target Section
#
$(TARGET): $(OBJS)
	$(CCLINK) -o $(TARGET) $(OBJS)


#
# File Section
#
main.o: main.c clinic.h
clinic.o: clinic.c clinic.h
doctor.o: doctor.c doctor.h
patient.o: patient.c patient.h defs.h


#
# Cleaning
#
clean:
	$(RM) $(TARGET) *.o *.bak *~"#"* core

            