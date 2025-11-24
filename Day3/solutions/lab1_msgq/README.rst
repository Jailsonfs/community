Lab 1: Data Passing — Message queue
===================================

Overview
********

In this lab, you will build a simple application that introduces the Zephyr
message queue. You will create a data passing flow between two threads using a
message queue.

Learning Objectives
*******************

By completing this lab, you will:

- Setup a message queue in Zephyr
- Implement a data passing flow in C

What You'll Implement
*********************

The starter project contains a basic structure. You will complete:

**main.c**
- Implement `cmd_hakuna()` and `cmd_matata()`
- Create a subcommand set with `SHELL_STATIC_SUBCMD_SET_CREATE`
- Register commands using `SHELL_CMD_REGISTER`

**prj.conf**
- Enable shell and UART backend


Results should be like
**********************

Console output:

    *** Booting Zephyr OS build v4.2.1 ***
    Consumer thread is running
    Filter thread is running
    Producer thread is running
    xxx Data 996 is invalid
    xxx Data 800 is invalid
    --> Consumed data: 32
    xxx Data 948 is invalid
    --> Consumed data: 164
    --> Consumed data: 268
    xxx Data 580 is invalid
    xxx Data 668 is invalid
    --> Consumed data: 152
    --> Consumed data: 388

