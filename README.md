# CBT619
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 619 is from Brian Westerman and contains the Dynamic      *   FILE 619
//*           Proclib modification, fitted to the Hercules MVS 3.8J *   FILE 619
//*           Turnkey #3 system.                                    *   FILE 619
//*                                                                 *   FILE 619
//*       Some of the members of this pds are in TSO XMIT format,   *   FILE 619
//*       which may cause a small amount of difficulty with an      *   FILE 619
//*       MVS 3.8J system, unless you know how to use Jim           *   FILE 619
//*       Morrison's XMIT370 and RECV370 programs (see File 571).   *   FILE 619
//*       Or you might want to download these members to a pc,      *   FILE 619
//*       and use the XMIT-manager program (available from a link   *   FILE 619
//*       at www.cbttape.org) to look at the $SMPLIST at least.     *   FILE 619
//*                                                                 *   FILE 619
//*       The modification allows execution of JCL which looks      *   FILE 619
//*       like this:                                                *   FILE 619
//*                                                                 *   FILE 619
//*  //BRIAN    JOB (ASSEMBLY),'SYSTEMS*BRIAN',CLASS=A,MSGCLASS=A,  *   FILE 619
//*  //         NOTIFY=BRIAN                                        *   FILE 619
//*  //JOBPROC  DD DISP=SHR,DSN=MY.PROC.LIBRARY,SYSPROC=YES         *   FILE 619
//*  //STEP1    EXEC  MYPROC                                        *   FILE 619
//*  /*                                                             *   FILE 619
//*                                                                 *   FILE 619
//*     This will cause the converter to first look in              *   FILE 619
//*     "MY.PROC.LIBRARY" for the procedure "MYPROC" and if not     *   FILE 619
//*     found there, it will then search the normal JES2            *   FILE 619
//*     concatenation.  If you had changed the 'SYSPROC=YES' to     *   FILE 619
//*     'SYSPROC=NO', then the search for the procedure "MYPROC"    *   FILE 619
//*     would have ended with the search of 'MY.PROC.LIBRARY',      *   FILE 619
//*     and if not found, a JCL error would have resulted.          *   FILE 619
//*                                                                 *   FILE 619
//*     Brian Westerman                                             *   FILE 619
//*     email: brian_westerman@syzygyinc.com                        *   FILE 619
//*     (800) 767-2244                                              *   FILE 619
//*     (800) 366-4082  - FAX                                       *   FILE 619
//*                                                                 *   FILE 619
```
