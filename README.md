# Dynamic Repair of Mission-Critical Applications with Runtime Snap-Ins
Sample code for runtime snap-ins, based on our paper

This is a prototype solution to provide reliable, non-disruptive updates to critical systems by a novel design pattern we call a snap-in, a method to install replacement routines embedded in one or more shared libraries while the system is running. 

Snap-ins take the approach of using the Linux ELF ABI to first load shared libraries containing replacement routines into a running application, supplanting the original routines with repaired ones without having to modify the existing code. The current version works with x86 platforms.

We provide an automated toolkit to scan application binaries and solve where to add the replacement routines. There are sample solutions included to help see how to create your own snap-ins.
