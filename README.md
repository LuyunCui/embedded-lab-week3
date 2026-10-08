# Embedded Systems — Week 3 Lab 2
Name: Lu Yuncui
Hardware Platform: FRDM-KL28Z
Lab Topic: GPIO Digital Output and State Machine Introduction

## Lab Objectives
1. Understand digital output implementation with GPIO peripherals.
2. Master the state transition model and implement state machines in C within a main loop.
3. Learn project compilation, download and debugging. Use breakpoints to inspect assembly code and variables.

## Completed Tasks
### Activity 1: Clone, compile and run the sample project
Successfully clone the initial source code, compile and download firmware to FRDM-KL28Z. Verify RGB LED works normally. Confirm the program is stored in Flash and remains after power cycle.

### Activity 2: Program Debugging
Set breakpoints and perform single-step debugging. Inspect assembly instructions corresponding to C source code. Locate the memory address of the instruction that turns on the green LED.

### Activity 3: 7-colour RGB cycle state machine (Demonstration Task)
Implement a 7-state state machine to cycle through all 7 RGB colours:
- Primary colours (Red, Green, Blue): hold for 2 seconds each
- Mixed colours (Cyan, Magenta, Yellow, White): hold for 1 second each
- Full cycle duration: 10 seconds, repeating infinitely

### Activity 4: Version Control
Commit source code locally, push changes to the remote GitHub repository and update this README file to document lab progress.

### Activity 5: Lightweight Multi-tasking with State Machines (Demonstration Task)
On bare-metal hardware without an operating system, use SysTick timer and state machines to implement two independent LED blink tasks.
The two LEDs have separate on/off timing and run in parallel inside one main loop, with no blocking delay functions.

### Activity 6: Multi-task Timing Debugging
Set breakpoints to observe state switching events of both tasks. Verify that the timing period of one task is not affected by the other.

### Activity 7: Lab Summary and Quiz
Complete the formative quiz for this lab. Document experimental observations, code logic and debugging experience.
