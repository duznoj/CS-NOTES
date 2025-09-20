
Red filled circle 🔴 = Enabled breakpoint
Red outlined hollow circle ⭕= Disabled Breakpoint

Clicking on a breakpoint gives 2 options:
1. Enable/Disable
2. Settings for advanced conditional breakpoints

Under "Debug" menu choose "Start Debugging" or Press F5 to start debugging
When execution reaches a Breakpoint, it stops, the line of the Breakpoint is NOT executed
And an arrow appears on the circle of the breakpoint to indicate that execution stopped here

Pressing F5 again/continue will continue the execution of program till it either terminates or a Breakpoint occurs


The Red Square forcefully terminates the program (Shift + F5)
The Reload button restarts the entire program (Ctrl + Shift + F5)

There are 3 ways to step through code once a Breakpoint is reached
##### Step Into (F11): 
This indicates that if the current line is a function, the debugger should step into the function

##### Step Over (F10):
This indicates that if the current line is a function, the debugger should allow the function to run to completion, and break at the next code after the function is done

##### Step Out (Shift + F11):
This indicates that the debugger should run until the current called function returns to the caller function

