AM_CFLAGS = -D_ANSC_LINUX
AM_CFLAGS += -D_ANSC_USER
AM_CFLAGS += -D_ANSC_LITTLE_ENDIAN_
AM_LDFLAGS = -L$(top_srcdir)/../CcspCommonLibrary/lib
AM_LDFLAGS += -lccsp_common

AM_CPPFLAGS = -Wall -Werror
ACLOCAL_AMFLAGS = -I m4
hardware_platform = i686-linux-gnu
bin_PROGRAMS = CcspLMLite
CcspLMLite_CPPFLAGS = -I$(CCSP_INSTALL_ROOT)/include/dbus-1.0 -I$(CCSP_INSTALL_ROOT)/lib/dbus-1.0/include -I$(top_srcdir)/../CcspCommonLibrary/source/ccsp/custom -I$(top_srcdir)/../CcspCommonLibrary/source/ccsp/include -I$(top_srcdir)/../CcspCommonLibrary/source/debug_api/include -I$(top_srcdir)/../CcspCommonLibrary/source/cosa/include -I$(top_srcdir)/../CcspCommonLibrary/source/cosa/include/linux -I$(top_srcdir)/../CcspCommonLibrary/source/ccsp/components/include -I$(top_srcdir)/../CcspCommonLibrary/source/cosa/package/slap/include -I$(top_srcdir)/../CcspCommonLibrary/source/util_api/http/include -I$(top_srcdir)/../CcspCommonLibrary/source/util_api/ansc/include -I$(top_srcdir)/../CcspCommonLibrary/source/ccsp/components/common/MessageBusHelper/include -I$(top_srcdir)/../hal/include $(CPPFLAGS)
CcspLMLite_SOURCES = lm_wrapper_priv_pc.c lm_api_test.c lm_main.c lm_wrapper.c lm_util.c
CcspLMLite_LDFLAGS =  -L$(top_srcdir)/../CcspCommonLibrary/lib -lccsp_common -L$(CCSP_INSTALL_ROOT)/lib -llmapi -lssl -lcrypto -lpthread -ldl

lib_LTLIBRARIES=liblmapi.la
liblmapi_la_CPPFLAGS= -D_ANSC_LINUX -D_ANSC_USER -D_ANSC_LITTLE_ENDIAN_ -I$(CCSP_INSTALL_ROOT)/include/dbus-1.0 -I$(CCSP_INSTALL_ROOT)/lib/dbus-1.0/include -I$(top_srcdir)/../CcspCommonLibrary/source/ccsp/custom -I$(top_srcdir)/../CcspCommonLibrary/source/ccsp/include -I$(top_srcdir)/../CcspCommonLibrary/source/debug_api/include -I$(top_srcdir)/../CcspCommonLibrary/source/cosa/include -I$(top_srcdir)/../CcspCommonLibrary/source/cosa/include/linux -I$(top_srcdir)/../CcspCommonLibrary/source/ccsp/components/include -I$(top_srcdir)/../CcspCommonLibrary/source/cosa/package/slap/include -I$(top_srcdir)/../CcspCommonLibrary/source/util_api/http/include -I$(top_srcdir)/../CcspCommonLibrary/source/util_api/ansc/include -I$(top_srcdir)/../CcspCommonLibrary/source/ccsp/components/common/MessageBusHelper/include
liblmapi_la_LDFLAGS= -L$(top_srcdir)/../CcspCommonLibrary/lib -lccsp_common
liblmapi_la_SOURCES= lm_api.c
liblmapi_la_DEPENDENCIES=
liblmapi_la_LIBADD=$(liblmapi_la_DEPENDENCIES)
