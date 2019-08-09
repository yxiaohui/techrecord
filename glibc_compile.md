- When do make, you may meet "can't be versioned to common symbol 'loc1'" problem.
-- vim $[you GLIBC dir]/misc/regexp.c
Change 
  char *loc1;
to
  char *loc1 __attribute__ ((nocommon));
