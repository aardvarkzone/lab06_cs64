README.txt (10 points)
The README should answer the following questions about your code.
Explain what you think the MIPs code is doing in a paragraph (3+ lines). 
Sufficiently summarizing what’s happening in your MIPs code’s disaggregate function 
is what we expect. Do not guess what the C/C++ code is doing. (5 points)

The MIPs code creates the buffer with the provided code and stores values of the 
array on different areas of the buffer depending on if the value is greater or
less than the average of the input array. Each section of the buffer of
consecutive values in memory is a smaller array that is then run through the
algorithm until the length of the array returned is 1 or the depth is 0. The 
recursive calls work in such a way that the array containing smaller values is 
passed through the function before the bigger array. 

Will the space used in the stack change with change in array length or change in 
array values? Or change in depth value? Why or why not? (5 points)

The stack usage is based on depth because everytime the function calls itself,
the stack has to allocate more memory. The number of function calls is based 
on the depth. 
