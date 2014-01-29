ACLOCAL_AMFLAGS = -I ../fintp_utils/m4

bin_PROGRAMS = EventsWatcher

AM_CPPFLAGS = -DUNIX -DDEBUG_ENABLED -DXALAN_1_9	\
@CPPFLAGS@	\
@PTHREAD_CFLAGS@	\
@XERCES_CPPFLAGS@ \
@XALAN_CPPFLAGS@	\
-I$(FINTP_HOME)/fintp_utils/src	\
-I$(FINTP_HOME)/fintp_log/src	\
-I$(FINTP_HOME)/fintp_transport/src	\
-I$(FINTP_HOME)/fintp_udal/src	\
-I$(FINTP_HOME)/fintp_base/src -I$(FINTP_HOME)/fintp_base/src/DB

AUTOMAKE_OPTIONS = foreign

EventsWatcher_LDFLAGS = @LDFLAGS@ @LIBS@	\
@PTHREAD_LIBS@ \
@XERCES_LDFLAGS@ -lxerces-c 	\
@XALAN_LDFLAGS@ -lxalan-c	\
-L$(FINTP_HOME)/fintp_utils/.libs -lfintp_utils	\
-L$(FINTP_HOME)/fintp_log/.libs -lfintp_log	\
-L$(FINTP_HOME)/fintp_transport/.libs -lfintp_transport	\
-L$(FINTP_HOME)/fintp_udal/.libs -lfintp_udal	\
-L$(FINTP_HOME)/fintp_base/.libs -lfintp_base

EventsWatcher_SOURCES = src/EventsWatcher.cpp	\
src/EventsWatcher.h	\
src/EventsWatcherDbOp.cpp	\
src/EventsWatcherDbOp.h	\
src/EventsWatcherMain.cpp	\
src/EventsWatcherMain.h	\
src/VersionInfo.cpp
