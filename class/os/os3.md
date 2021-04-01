---
date: 2021-03-19T20:32
title: os3
slug: os
tags:
  - os
---

# Program and Process

## BackGround
- Program load as Proscess
- But Process there's only one, in memory
- jumlah core di cpu terbatas
- Jumlah process melebihi jumlah core
- Hardware resource have to used efficientlly

## Program
- Collection of Instruction run by cpu
- Executable Program has been assigned virtual adress by the linker stage of compilation
  process
- OS loader reads the executable program

## Process
- Process is an instance of program, set 
- new process not made from scratch but clone it and fork()

## PCB (Process Control Block)
- PCB is where CPU context is stored for any process not currently excute by cpu
### Parent and child
- all process have parent except init
- each pcb have pointer to parent process

## Switching Process
- Each process has a context
  - 

### xv6 context switch

## Executing a program
- exec() replace current process image with a new one
- in Linux exec() is part of c library

## Loader in Linux

## Mode Transfer sequence
