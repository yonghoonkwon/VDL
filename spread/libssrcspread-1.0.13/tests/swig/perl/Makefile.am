## Copyright 2006 Savarese Software Research Corporation
##
## Licensed under the Apache License, Version 2.0 (the "License");
## you may not use this file except in compliance with the License.
## You may obtain a copy of the License at
##
##     http://www.savarese.com/software/ApacheLicense-2.0
##
## Unless required by applicable law or agreed to in writing, software
## distributed under the License is distributed on an "AS IS" BASIS,
## WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
## See the License for the specific language governing permissions and
## limitations under the License.

include $(top_srcdir)/config/global.mk

if LIBSSRCSPREAD_SWIG
if LIBSSRCSPREAD_PERL

export PERL5LIB = ./ssrc
export LIBSSRCSPREAD_TEST_DAEMON = $(libssrcspread_test_daemon)

TESTS = ErrorTest.pl GroupListTest.pl MessageTest.pl MailboxTest.pl
EXTRA_DIST = $(TESTS)
check_SCRIPTS = $(TESTS)

ssrc:
	$(LN_S) $(top_builddir)/swig/perl ssrc

$(TESTS): ssrc

endif
endif
