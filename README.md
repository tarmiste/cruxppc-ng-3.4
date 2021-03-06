# cruxppc-ng-3.4

01Feb2019

## CRUX 3.4 port to powerpc (32bit)

  This repository contains a port of CRUX Linux 3.4 to the PowerPC architecture (32 bit only).   

  Note that this project is not a part of, nor sponsored, nor endorsed by the 
mainline CRUX project.  If you are using CRUX-PPC and run into problems, please do not ask questions or raise issues against the mainline CRUX project.  

  CRUX is a lightweight Linux distribution and CRUX PPC is an even lighter weight port of CRUX to the PowerPC architecture.   CRUX provides 
  a small set of prebuilt packages which are sufficient to get started with but most CRUX packages will have to be built and added by the user.   If you are 
  looking for a turn key Linux distro for your hardware with many prebuilt packages available, CRUX is not what you are looking for.   
  
  CRUX provides a minimal starting root filesystem and the user then builds and adds additional packages as they desire.   CRUX is a build it yourself and 
  figure it out yourself kind of distribution.   CRUX users will need to be comfortable working with the command line, editing configuration files,
  building packages, etc.   If you desire point and click system maintenance, CRUX is not what you are looking for.

  CRUX-PPC supports 32bit PowerPC G3 and G4.   It does not support 64bit PowerPC (G5) at this time.   There are still a fair number of Linux distributions supporting G5 machines but distros supporting 32bit PowerPC are getting scarce.  Hence, for now, CRUX-PPC is focused on the 32bit PowerPC machines.

  This project is not a continuation of the (now defunct) CRUX-PPC project which existed previously (until 2012 or so).   This project is a 
  new port of CRUX-3.4 to the PowerPC.  Although similarities exist and pieces from the previous CRUX-PPC may be reused in this project, this is a
  fresh port of CRUX to the PowerPC and backwards compatibility with the previous CRUX PPC is not a goal of this project.

  crux ppc 3.4 is a work in progress.  It still has a lot of rough edges.
If you are already familiar with CRUX or manual installation and configuration
of a Linux sytem, then you should be able to work through the rough spots.
As time passes, the rough edges will be smoothed out but as of right now,
it will be a difficult distribution for some.


### Contents:

  This repository provides the crux core, opt and xorg ports that are
known to require changes to work for the powerpc.  These can be found 
in the 'core-ppc', 'opt-ppc' and 'xorg-ppc' directories.  Ports which
are unchanged for powerpc are not included in this directory but instead
are sourced from the main (x86/64) crux project.

  This repository provides release notes, an installation handbook
and various notes and materials related to crux ppc development.

  The 'releases' section of this repository provides a starter 
crux ppc 3.4 root filesystem.  This rootfs is the seed from which a user
grows the remainder of their crux system.

  Of course this README file and various other information.


### Usage overview:

  Download the root filesystem tarball.   

  The user extracts the root filesystem into the partition or directory 
  that will contain the crux ppc system.

  The user will need to build a number of additional packages to have 
  a fully functional crux system.   At the least, the packages openssl,
  ca-certificates, and wget will have to be built to support automatic
  download and building of packages with the crux package utilities.

  If bootable crux system is desired, the user will build the kernel 
  and configure the bootloader to boot the crux system.   A sample 
  kernel configuration file is provided (under kernel) that may be 
  helpful in creating the kernel.

  A more detailed description of installing and configuring CRUX PPC can be
  found in the handbook and release notes.
