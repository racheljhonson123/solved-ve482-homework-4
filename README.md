Download Link: https://assignmentchef.com/product/solved-ve482-homework-4
<br>
<h1><strong>Ex. 1 — </strong>Simple questions</h1>

<ol>

 <li>Consider a system in which threads are implemented entirely in user space, with the run-time system getting a clock interrupt once a second. Suppose that a clock interrupt occurs while some thread is executing in the run-time system. What problem might occur? Can you suggest a way to solve it?</li>

 <li>Suppose that an operating system does not have anything like the select system call (man select for more details on the command) to see in advance if it is safe to read from a file, pipe, or device, but it does allow alarm clocks to be set that interrupt blocked system calls. Is it possible to implement a threads package in user space under these conditions? Discuss.</li>

</ol>

<h1><strong>Ex. 2 — </strong>Monitors</h1>

During the lecture monitors were introduced (3.30). They use condition variables as well as two instructions, wait and signal. A different approach would be to have only one operation called waituntil, which would check the value of a boolean expression and only allow a process to run when it evaluates as True. What would be the drawback of such a solution?

<h1><strong>Ex. 3 — </strong>Race condition in Bash</h1>

Write a Bash script which generates a file composed of one integer per line. The script should read the last number in the file, add one to it, and append the result to the file.

<ol>

 <li>Run the script in both background and foreground at the same time. How long does it take before observing a race condition?</li>

 <li>Modify the script such as to prevent the race condition.</li>

</ol>

<h1><strong>Ex. 4 — </strong>Programming with semaphores</h1>

The following C code creates two threads which increment a common global variable. When run it generates a random and inaccurate output. In order to solve this problem we want to use semaphores.

<ol>

 <li>On Linux, find the file <em>h</em>.</li>

 <li>Read the documentation to understand how to use the functions described in the file <em>h</em>.</li>

 <li>Using semaphores adjust the program such as to always return the correct answer.</li>

</ol>