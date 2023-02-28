# PROBLEM-STATEMENT
 GROUP ASSIGNMENT
The code defines a base class named "StopwatchBase" and a derived class named "Stopwatch". 
The base class defines four virtual functions: start(), stop(), reset(), and displayTime(), which are meant to be implemented by any derived class inheriting from it.
The derived class "Stopwatch" implements these four virtual functions. It contains a private member variable of type "steady_clock::time_point" to keep track of the start time and end time of the stopwatch. It also has a boolean variable named "isRunning" to indicate whether the stopwatch is currently running or not.
In the main function, an object of type "Stopwatch" is created. 
The "start()" function is called to start the stopwatch, then the thread is paused for 2 seconds using "this_thread::sleep_for(chrono::seconds(2))".
After that, the "stop()" function is called to stop the stopwatch, and the "displayTime()" function is called to print the elapsed time since the stopwatch was started.
Then, the "reset()" function is called to reset the stopwatch, and the same process is repeated again, but this time the thread is paused for 1 second before stopping the stopwatch and displaying the elapsed time.
Overall, the code simulates a stopwatch by measuring the time elapsed between the "start()" and "stop()" calls and displaying the result.
