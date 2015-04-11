Data Analyzing
========


Sending and Receiving
---

  * After executing the `tcl` program, you can type the following command in your Linux terminal. It will create a file named `tcp.tr`, which contains the details of the package that we send and receive.
  This command allow you to check the package numbers that we receive.
  ```
  grep "^r" simple.tr | grep "tcp" | grep "_1_ AGT" > tcp.tr
  ```
  This command allow you to check the package numbers that we send.
  ```
  grep "^s" simple.tr | grep "tcp" | grep "_0_ RTR" > tcp.tr
  ```
  You can get the exact package numbers by counting how many lines there are in the `tcp.tr` file.

  * We have **already counted it**, so you don't have to do it again.

  > **DSDV**
  5424(send)    5402(receive)

  > **AODV**
  4666(send)    4665(receive)

  > **DSR**
  6920(send)    6919(receive)

Result Graph
---
  * You can get the files from the `img` directory.
