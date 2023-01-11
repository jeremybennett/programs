
[comment]: # "this template is for ARVM projects"

# **ARVM-FunctionalCoverage** Monthly Report for 17-October-2022

Project leader : Simon Davidmann   
Lead company :  Imperas  
Participating companies : SiLabs, Dolphin  

## Overview
There are almost 1,000 instructions in RV64 (inc. all ratified and soon to be ratified extensions).  
For each instruction somebody will need to write SystemVerilog covergroups and coverpoints…   
Maybe 10-40 lines of SystemVerilog for each instruction…   
That is 10,000-40,000 lines of SystemVerilog code to be written… (and be correct and working…)  
And that is just for the basic un-privilege mode ISA…   

This sub-project is to enable the developing of open-source VIPs (such as functional coverage) that can be used for many different core configurations/implementations.  

## Current Status
cv32e40p used first generation of SystemVerilog for RV32I generated by Imperas in 2020.  
Second generation architecture is generated and works directly from RVVI-TRACE core tracer testbench interface.   
Uses machine readable ISA definition and generates examples as compliance level functional coverage for RV32I, RV32M.   
Currently soliciting input / requirements on what needs to be covered in verification plans for different ISA extensions.   
Initial focus is F (FPU) functional coverage for cv32e40pv2 (Dolphin) and Zc for cv32e40s (SiLabs).   

## Key activities / tasks completed this month
- Topic presented (Oct. 4th) at DVClub Europe/India webinar: https://www.tessolve.com/automated-verification-checks/
- F (FPU): First SystemVerilog functional coverage code for FPU has been generated and is under review at Dolphin
- Zc (code-size-reduction): has been coded up into machine readable form and is soon to be generated  
- existing generated code is under review in SiLabs 
- output of code generator is sections for verification plan in .csv - currently being reviewed  

## Planned activities / tasks for coming month
- reviews of resultant functional coverage (RV32I, RV32M, F, Zc)   
- addition of more requirements for F and Zc
- addition of more design verification (DV) coverage such as hazards (and micro-architectural)   
- scheduling of regular sub-project progress meetings (currently they are ad-hoc)  
- discussions regarding working with isacov

## Issues / items that are slowing progress
- none - just starting up...

