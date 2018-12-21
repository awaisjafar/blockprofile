# BlockProfile : Profiling in C

The profiler contains helper functions in order to calculate how much time is elapsed ( Wall Clock Time ) for a given piece of code. Main modules of this library are as following

- <span style="color:blue">time_start( label )</span> -  Starting the measurement of execution time for the block starting with “label”
- <span style="color:blue">time_end( label )</span>  -  End of the block initialized with time_start() function having the tag “label”
- <span style="color:blue">total_time(  )</span>  -  The total amount of time for all the blocks combines. Return type of this is float
- <span style="color:blue">time_summary(  )</span> - Total time for each individual execution block labelled
- <span style="color:blue">elapsed_time( label )</span>  -  Total time of execution for the block having tag “label”

 Just include the profile.c file in your code.

## Example 

 example.c is an exmaple piece of code that calculate the Fobinacci numbers from 1 to 43. In the end, time_summary is called to print all the modules with their corresponding wall clock times.

 **Note:** This module doesn't take any different considerations for the Overlapping blocks