Completing the Program (15 points)
This program prints a table of runtimes (these are displayed in seconds) for given functions
on arrays.

The program tests different array sizes to establish a relationship between input size and
runtime. It tests each array size multiple times and then takes an average of the times. We
also output how much the average runtime increased relative to the previous average. This
is calculated by dividing the current average by the previous average (output “N/A” for the
first increase value).

Here are example calls to the timing functions:
      functionRuntimes fRT;
      int sizes1[] = { 2000, 4000, 8000, 16000, 32000, 64000, 128000, 256000};
      
      srand(time(0));
      
      fRT = timeAlgorithm("Insertion Sort", 6, 5, sizes1, insertionSortInitial );
      printRuntimeTable(fRT);
      freeFunctionRuntimes(fRT);
      
      fRT = timeAlgorithm("quicksort", 12, 8, sizes1, quickSortOptInitial );
      printRuntimeTable(fRT);
      freeFunctionRuntimes(fRT);
      
The runtimes are stored in a functionRuntimes struct. You are completing a program to create and fill data in this struct, print the data of this struct, and free this struct.

After you have the program completed, you should use it to help determine the asymptotic runtimes of the three mystery functions (i.e., mysteryRuntime1, mysteryRuntime2, mysteryRuntime3).
Be sure to also examine the code of the mystery functions to confirm/improve your estimations.
Fill in the following table in the provided file:

     /*
     TODO: Give your asymptotic estimates for the runtimes of the following 3 functions:
     mysteryRuntime1: O( )
     mysteryRuntime2: O( )
     mysteryRuntime3: O( )
     */
