# This file was automatically generated by bakefile.
#
# Any manual changes will be lost if it is regenerated,
# modify the source .bkl file instead if possible.

# You may define standard make variables such as CFLAGS or
# CXXFLAGS to affect the build. For example, you could use:
#
#      make CXXFLAGS=-g
#
# to build with debug information. The full list of variables
# that can be used by this makefile is:
# AR, CC, CFLAGS, CPPFLAGS, CXX, CXXFLAGS, LD, LDFLAGS, MAKE, RANLIB.

# You may also specify config=Debug|Release
# or their corresponding lower case variants on make command line to select
# the corresponding default flags values.
ifeq ($(config),debug)
override config := Debug
endif
ifeq ($(config),release)
override config := Release
endif
ifeq ($(config),Debug)
CPPFLAGS ?= -DDEBUG
CFLAGS ?= -g -O0
CXXFLAGS ?= -g -O0
LDFLAGS ?= -g
else ifeq ($(config),Release)
CPPFLAGS ?= -DNDEBUG
CFLAGS ?= -O2
CXXFLAGS ?= -O2
else ifneq (,$(config))
$(warning Unknown configuration "$(config)")
endif
#
# Additionally, this makefile is customizable with the following
# settings:
#
#      ITTIA_DB_HOME  Path to ITTIA DB SDK

# Use "make RANLIB=''" for platforms without ranlib.
RANLIB ?= ranlib

CC := cc
CXX := c++

# The directory for the build files, may be overridden on make command line.
builddir = .


# ------------
# Configurable settings:
# 

# Path to ITTIA DB SDK
ITTIA_DB_HOME ?= /opt/ittiadb

# ------------

all: builddir-error-handling ../../$(builddir)/src/error_handling/transaction_rollback_c ../../$(builddir)/src/error_handling/savepoint_rollback_c

builddir-error-handling:
	@mkdir -p ../../$(builddir)/src/error_handling

../../$(builddir)/src/error_handling/transaction_rollback_c: ../../$(builddir)/src/error_handling/transaction_rollback_c_main.o ../../$(builddir)/src/error_handling/transaction_rollback_c_db_main.o ../../$(builddir)/src/error_handling/transaction_rollback_c_dbs_schema.o ../../$(builddir)/src/error_handling/transaction_rollback_c_dbs_error_info.o ../../$(builddir)/src/error_handling/transaction_rollback_c_transaction_rollback.o ../../$(builddir)/src/error_handling/transaction_rollback_c_db_schema.o
	$(CXX) -o $@ $(LDFLAGS) ../../$(builddir)/src/error_handling/transaction_rollback_c_main.o ../../$(builddir)/src/error_handling/transaction_rollback_c_db_main.o ../../$(builddir)/src/error_handling/transaction_rollback_c_dbs_schema.o ../../$(builddir)/src/error_handling/transaction_rollback_c_dbs_error_info.o ../../$(builddir)/src/error_handling/transaction_rollback_c_transaction_rollback.o ../../$(builddir)/src/error_handling/transaction_rollback_c_db_schema.o -L$(ITTIA_DB_HOME)/lib -littiasql -pthread

../../$(builddir)/src/error_handling/transaction_rollback_c_main.o: ../common/main.c
	$(CC) -c -o $@ $(CPPFLAGS) $(CFLAGS) -MD -MP -pthread -I$(ITTIA_DB_HOME)/include -I../common -I$(ITTIA_DB_HOME)/share/doc/ittiadb/examples ../common/main.c

../../$(builddir)/src/error_handling/transaction_rollback_c_db_main.o: ../common/db_main.c
	$(CC) -c -o $@ $(CPPFLAGS) $(CFLAGS) -MD -MP -pthread -I$(ITTIA_DB_HOME)/include -I../common -I$(ITTIA_DB_HOME)/share/doc/ittiadb/examples ../common/db_main.c

../../$(builddir)/src/error_handling/transaction_rollback_c_dbs_schema.o: $(ITTIA_DB_HOME)/share/doc/ittiadb/examples/dbs_schema.c
	$(CC) -c -o $@ $(CPPFLAGS) $(CFLAGS) -MD -MP -pthread -I$(ITTIA_DB_HOME)/include -I../common -I$(ITTIA_DB_HOME)/share/doc/ittiadb/examples $(ITTIA_DB_HOME)/share/doc/ittiadb/examples/dbs_schema.c

../../$(builddir)/src/error_handling/transaction_rollback_c_dbs_error_info.o: $(ITTIA_DB_HOME)/share/doc/ittiadb/examples/dbs_error_info.c
	$(CC) -c -o $@ $(CPPFLAGS) $(CFLAGS) -MD -MP -pthread -I$(ITTIA_DB_HOME)/include -I../common -I$(ITTIA_DB_HOME)/share/doc/ittiadb/examples $(ITTIA_DB_HOME)/share/doc/ittiadb/examples/dbs_error_info.c

../../$(builddir)/src/error_handling/transaction_rollback_c_transaction_rollback.o: transaction_rollback.c
	$(CC) -c -o $@ $(CPPFLAGS) $(CFLAGS) -MD -MP -pthread -I$(ITTIA_DB_HOME)/include -I../common -I$(ITTIA_DB_HOME)/share/doc/ittiadb/examples transaction_rollback.c

../../$(builddir)/src/error_handling/transaction_rollback_c_db_schema.o: db_schema.c
	$(CC) -c -o $@ $(CPPFLAGS) $(CFLAGS) -MD -MP -pthread -I$(ITTIA_DB_HOME)/include -I../common -I$(ITTIA_DB_HOME)/share/doc/ittiadb/examples db_schema.c

../../$(builddir)/src/error_handling/savepoint_rollback_c: ../../$(builddir)/src/error_handling/savepoint_rollback_c_main.o ../../$(builddir)/src/error_handling/savepoint_rollback_c_db_main.o ../../$(builddir)/src/error_handling/savepoint_rollback_c_dbs_schema.o ../../$(builddir)/src/error_handling/savepoint_rollback_c_dbs_error_info.o ../../$(builddir)/src/error_handling/savepoint_rollback_c_savepoint_rollback.o ../../$(builddir)/src/error_handling/savepoint_rollback_c_db_schema.o
	$(CXX) -o $@ $(LDFLAGS) ../../$(builddir)/src/error_handling/savepoint_rollback_c_main.o ../../$(builddir)/src/error_handling/savepoint_rollback_c_db_main.o ../../$(builddir)/src/error_handling/savepoint_rollback_c_dbs_schema.o ../../$(builddir)/src/error_handling/savepoint_rollback_c_dbs_error_info.o ../../$(builddir)/src/error_handling/savepoint_rollback_c_savepoint_rollback.o ../../$(builddir)/src/error_handling/savepoint_rollback_c_db_schema.o -L$(ITTIA_DB_HOME)/lib -littiasql -pthread

../../$(builddir)/src/error_handling/savepoint_rollback_c_main.o: ../common/main.c
	$(CC) -c -o $@ $(CPPFLAGS) $(CFLAGS) -MD -MP -pthread -I$(ITTIA_DB_HOME)/include -I../common -I$(ITTIA_DB_HOME)/share/doc/ittiadb/examples ../common/main.c

../../$(builddir)/src/error_handling/savepoint_rollback_c_db_main.o: ../common/db_main.c
	$(CC) -c -o $@ $(CPPFLAGS) $(CFLAGS) -MD -MP -pthread -I$(ITTIA_DB_HOME)/include -I../common -I$(ITTIA_DB_HOME)/share/doc/ittiadb/examples ../common/db_main.c

../../$(builddir)/src/error_handling/savepoint_rollback_c_dbs_schema.o: $(ITTIA_DB_HOME)/share/doc/ittiadb/examples/dbs_schema.c
	$(CC) -c -o $@ $(CPPFLAGS) $(CFLAGS) -MD -MP -pthread -I$(ITTIA_DB_HOME)/include -I../common -I$(ITTIA_DB_HOME)/share/doc/ittiadb/examples $(ITTIA_DB_HOME)/share/doc/ittiadb/examples/dbs_schema.c

../../$(builddir)/src/error_handling/savepoint_rollback_c_dbs_error_info.o: $(ITTIA_DB_HOME)/share/doc/ittiadb/examples/dbs_error_info.c
	$(CC) -c -o $@ $(CPPFLAGS) $(CFLAGS) -MD -MP -pthread -I$(ITTIA_DB_HOME)/include -I../common -I$(ITTIA_DB_HOME)/share/doc/ittiadb/examples $(ITTIA_DB_HOME)/share/doc/ittiadb/examples/dbs_error_info.c

../../$(builddir)/src/error_handling/savepoint_rollback_c_savepoint_rollback.o: savepoint_rollback.c
	$(CC) -c -o $@ $(CPPFLAGS) $(CFLAGS) -MD -MP -pthread -I$(ITTIA_DB_HOME)/include -I../common -I$(ITTIA_DB_HOME)/share/doc/ittiadb/examples savepoint_rollback.c

../../$(builddir)/src/error_handling/savepoint_rollback_c_db_schema.o: db_schema.c
	$(CC) -c -o $@ $(CPPFLAGS) $(CFLAGS) -MD -MP -pthread -I$(ITTIA_DB_HOME)/include -I../common -I$(ITTIA_DB_HOME)/share/doc/ittiadb/examples db_schema.c

clean:
	rm -f *.o
	rm -f *.d
	rm -f ../../$(builddir)/src/error_handling/transaction_rollback_c
	rm -f ../../$(builddir)/src/error_handling/savepoint_rollback_c

.PHONY: all clean builddir-error-handling

# Dependencies tracking:
-include *.d
