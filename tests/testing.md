

## Testing notes.


Core package tests (i.e. "make check) usually passed but had some 
unexpected failures (e.g. every patch test failed).  After some hunting, 
figured out that the default shell is dash rather than bash
and some of the package tests assume a bash shell.  Tests
should be rerun with bash shell to get accurate results.

Pkgfiles usually don't have commands to execute test suites.  Tests
can be run manually. 

The glibc test-fenv test causes the testing to abort.   The tests can
be resumed after the abort and run to completion.  



