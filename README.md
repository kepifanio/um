# um
/******************************************************************************
*
* Filename: README
* By: Katherine Epifanio (kepifa01)
*     & Olivia Hayward 
* Date: 11/25/2020
* Assignment: Homework 6
*
******************************************************************************/

Architecture:
    um.c: Main driver for the program. Opens the .um file and calls the
        load_program function and execute_um function.
    um_load_program.c/.h: This file contains all of the functions for the
        initial setup of the UM. It determines the file size and creates new
        bitpacked instructions.
    um_execute.c/.h: This file contains all of our instruction functions
        besides those that deal with segments. It also holds our main function
        that reads and interprets the codewords.
    um_memory.c/.h: This file deals with all of the memory for our UM. It
        contains all of the segment-related functions and also initializes the
        memory for the mem_t struct and frees all the memory.

It takes our UM approximately 2.9329 seconds to complete 50
million instructions. We used the time function on the
command line to time our program completing midmark, which
is 85,070,522 instructions. It took our program 4.99 seconds
to complete that.
