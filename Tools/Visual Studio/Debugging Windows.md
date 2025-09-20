

## Autos
Shows the names and value, type of entities which have changed in the most recent execution.

## Locals
Shows the name, value, types of ALL variables in the current execution scope

## Watch (Most useful probably)
Watch windows can be used to either watch individual memory locations, variables, or expressions, and also CPU Registers

Eg: if there is a variable "n", we can see:
&n, n+10, etc

## Call Stack
Stack of function calls exactly as expected:
Top = function currently being executed

Below any function is the callee of that function

## Breakpoints
Show the current defined breakpoints, can be used to toggle a Breakpoint between Enable/Disable
Also can be used to add Conditional Breakpoints


#### --- Above are the default windows ---

## Memory

Can be added by going in the Debug Menu

Debug Menu -> Windows -> Memory -> Memory 1

Memory gives a view of the Virtual Memory (I think?).

We can jump to a variables memory by searching for its address. Eg: &<varName>.

Or by typing in an absolute address, Eg: 0x500000

Or to go to an address stored in a CPU register, write the name of the register. Eg: Address: RSP, now you're viewing the top of stack