# Debugging tips and tricks 


## Stack smashing and reverse debugging

How to use gdb to detect stack overflows problems

* Run the program util its crash 
`while <my-program>; do echo OK; done`

* I could do the same inside gdb
`gdb --args <my-program>`

* Add break points
`
 break main
 break _exit
`
*  Add recording command  
` command 1
  record
  continue`
* Add rerun command
` 
  command 2
  run
`
* Turn of the confirmations
` set confirm off`

* Run
`run`

* Examination 
`backtrace
 p $pc
 x $pc
`
* Return one step instruction
`reverse-stepi
disassemble
`
* Examine the stack pointer and watch it 
`p $sp
watch *(long*) <the value of $sp>`

* Reverse continue
`rc`



