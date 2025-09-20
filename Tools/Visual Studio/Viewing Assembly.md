
When stopped at a breakpoint:

1. Right click in the code display window -> Go To Disassebmly (or Ctrl+K, G)

In the "Viewing Disassembly" Mode,
The Autos Window will now display only the CPU Registers

#### View All Registers
Debug Menu -> Windows -> Registers
Right Click in the Registers Window to toggle which registers you want to see


To View the Stack, inside a [[Debugging Windows#Memory|Memory Window]]:
1. Go to memory address pointed by RSP
2. Set Columns to 1 in the Memory Window to see the stack Byte by Byte


In the Disassembly view of the code, you can see instructions like:

```
dword ptr [n], 0Ah
```

We are getting the symbol/variable name "n", this would happen only if we assembled/compiled using the -g flag to get the debugging symbols.
In the unknown/random binaries of other's programs we won't get these.

Therefore, to familiar ourselves better with this we'll disable symbol names by doing: Right Click in the "Disassembly" Window -> Toggle "Show Symbol Names" off

Now the Disassembly looks like:
```
dword ptr [rsp+24h], 0Ah
```
this means "n" is nothing but THE 4 byte or (sizeof (int)) number of bytes at the address rsp+24h.
i.e, 24h bytes below from the  top of the stack
This means its a local variable living on the stack