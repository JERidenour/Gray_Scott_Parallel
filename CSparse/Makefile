#------------------------------------------------------------------------------
# CSparse Makefile
#------------------------------------------------------------------------------

VERSION = 3.1.4

C:
	( cd Lib ; $(MAKE) )
	# ( cd Demo ; $(MAKE) )

# all: C cov
all: C

library:
	( cd Lib ; $(MAKE) )

# cov:
# 	( cd Tcov ; $(MAKE) )

clean:
	( cd Lib ; $(MAKE) clean )
	( cd Demo ; $(MAKE) clean )
	( cd Tcov ; $(MAKE) clean )
	( cd MATLAB/CSparse ; $(RM) *.o )
	( cd MATLAB/Test    ; $(RM) *.o )

purge:
	( cd Lib ; $(MAKE) purge )
	( cd Demo ; $(MAKE) purge )
	( cd Tcov ; $(MAKE) purge )
	( cd MATLAB/CSparse ; $(RM) *.o *.mex* )
	( cd MATLAB/Test    ; $(RM) *.o *.mex* )

distclean: purge

