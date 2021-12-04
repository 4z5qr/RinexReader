####################################################################
# Makefile for building the students application
#


#
# Definitions
#

CC = g++ -Wall -std=c++11
CFLAGS = g++ -Wall -std=c++11
CCLINK = $(CC)
OBJS = TimeUtils.o StringUtils.o FileIO.o pch.o Rinex3Obs.o Rinex3Nav.o Rinex2Obs.o Rinex2Nav.o RinexReader.o 
RM = rm -f
TARGET = RinexReader

#
# Target Section
#
$(TARGET): $(OBJS)
	$(CCLINK) -o $(TARGET) $(OBJS)


#
# File Section
#
RinexReader.o: RinexReader.cpp pch.h Rinex2Nav.h Rinex2Obs.h Rinex3Nav.h Rinex3Obs.h FileIO.h StringUtils.h
 
Rinex2Nav.o: Rinex2Nav.cpp Rinex2Nav.h
Rinex2Obs.o: Rinex2Obs.cpp Rinex2Obs.h
Rinex3Nav.o: Rinex3Nav.cpp Rinex3Nav.h
Rinex3Obs.o: Rinex3Obs.cpp Rinex3Obs.h
pch.o: pch.cpp pch.h
FileIO.o: FileIO.cpp FileIO.h
StringUtils.o: StringUtils.cpp StringUtils.h
TimeUtils.o: TimeUtils.cpp TimeUtils.h

#RinexReader123: RinexReader.o Rinex2Nav.o Rinex2Obs.o Rinex3Nav.o Rinex3Obs.o pch.o FileIO.o StringUtils.o

#
# Cleaning
#
clean:
	$(RM) $(TARGET) $(OBJS) *.o *.bak *~"#"* core