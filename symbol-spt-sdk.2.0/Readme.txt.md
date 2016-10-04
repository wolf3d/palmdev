##Readme file for Symbol Palm Terminal SDK Version 2.00 

###CONTENTS:

####1.0 Purpose of this release
####2.0 Directory structure of the Symbol Scanner SDK
####3.0 About the files in each subdirectory
####4.0 Special notes for this release


#####1.0 Purpose of this release

This release of the Symbol Scanner SDK is provided for use with 
version 3.0 of the Palm OS. It contains the SPT SDK files and
sample application code. The files contained in this SDK release are subject to change.

#####1.1 Readme files

See the individual readme files for printing, for the magnetic stripe
reader (msr) and for Spectrum24 (S24) to learn more about each of these products.

#####2.0  Directory structure of the Symbol Scanner SDK

Symbol SDK  		-  The main ScanManager directory
Symbol SDK\Document	-  Documentation in PDF format
Symbol SDK\Lib		-  Library files
Symbol SDK\Include	-  All header files
Symbol SDK\prc		-  Supporting prc and pdb files
Symbol SDK\Sample	-  Source for the SPT, printer, MSR 
				   and S24 applications
Symbol SDK\Host Tools
		\msr	-  Host MSR configurator


#####3.0 About the files in each sub directory

#####3.1 Symbol SDK\Document

The following documentation is included:

    ssm.pdf	- Symbol Palm Terminal Scanner System Software Manual
    psm.pdf	- Printer Software Manual for the Palm Computing Platform
    msrssm.pdf	- MSR 3000 System Software Manual
    s24api.pdf  - SPT 1740 Spectrum24 Driver Extensions Library 
                  Developer's Guide

The "Symbol Palm Terminal Scanner System Software Manual" provides the 
Documentation in PDF format for use when developing scan aware 
applications for the Symbol Palm Terminal (SPT).  

The "Printer Software Manual for the Palm Computing Platform" provides
documentation in PDF format for developing printer applications for the
SPT and PalmIII units.  

The "MSR 3000 System Software Manual" provides information for use in 
developing applications to enable magnetic stripe reading on the 
Symbol Technologies SPT 1740 Terminal.

The "SPT 1740 Spectrum24 Driver Extensions Library Developer's Guide " 
provides an overview of Spectrum24 wireless operation and information
about the Spectrum24 library functions that can be used by developers
for the SPT 1740.

#####3.2 Symbol SDK\Lib
The ScanMgr.lib file is linked with your source code and provides the 
interface to the Scan Manager Shared Library.  PtStatic.lib is the 
shared library that must be linked with your source code for printing. 
The library, SPT1740.lib, must be used for Spectrum24.

#####3.3 Symbol SDK\prc
The file MsrMgrLib.prc is the shared library needed for use and control 
of the MSR 3000.  

The two pdb files are used for printing. These two files, Printcap.pdb 
and ptDynLib.pdb must be HotSynced onto the SPT for printing, along with
the user application or PrintSample.prc (See sample subdirectory).

#####3.4 Symbol SDK\Sample
Source for the ScanDemo and SimpleScan applications. These applications
are supplied to help developers create scan aware applications using the 
Metrowerks Codewarrior IDE. It is expected that portions of this sample 
code will be used in developer applications. The SimpleScan application 
is designed to get the developer up and running quickly with simple scan 
aware applications, while ScanDemo is more advanced, showing the developer 
how to provide enhanced scan aware capabilities into their applications. 

The SimpleScan demo is completely described in Chapter 6 of the 
"Symbol Palm Terminal Scanner System Software Manual".

The source for PrintSample is provided as a example of how to use the
printer API.  See the readme file,readme_printing.txt, for additional
information about the print sample program and the printer API.  

Two examples demonstrating MSR ability are provided: MSR Demo and
MSR Sample. See the readme file,readme_msr.txt, for additional
information about the SPT Magnetic Stripe Reader. 

Examples for Spectrum24 code are provided in the S24 Samples Directory. 


#####4.0 Special notes for this release

#####4.1 Users should be able to generate the sample code for all demos using Metrowerks CodeWarrior.
