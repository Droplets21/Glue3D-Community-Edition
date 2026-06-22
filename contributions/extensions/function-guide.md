## A guide on how to use functions
### What are functions for?
Functions can be used to orginize and reuse large and small peices of code, they can be used to perform tasks or even return data.

### How do I make a function?
In the script editor, there is a button at the top on the toolbar labeled "function", on pressing that button a new function file will be crated. Once you've got a function, you can open it in the script editor and write you function!
> [!caution]
> When a function is made two blocks are there by default; `func.start` and `func.end`, make sure that any code you place are between those two lines, anything outside can have unwanted side effects

While your writing your function, you can use blocks like `func.read` and `func.return`, here is what they do:
1. `func.read(val input#)` reads one of four parameters the function gets (a parameter in this case is data you can send to a function when calling it), you won't recieve any data unless that parameter is actually set.
   
2. `func.return(str return)` returns data to the caller script, so if I had a function that added 1 and 2, I could use the return block to return the sum

### How do I call a function?
In the script you want to call the function in, you can use the `func.call(str name)` to call a function file with that name, along with calling, you can also set the parameters before you call, here is all the stuff you can work with when calling a function:
1. `func.inputs(str in1, str in2, str in3, str in4)` lets you set all 4 parameters in one line

2. `func,input1(val in#, str in)` sets only one parameter

Once you've called the function, you can use the `data_return` variable to read any return the function makes

## Things to note
Even though functions are stored the same way normal scripts are, you can't assign a function to an obj, functions are global, so you can call them in any script, though you may face some local variable issues/
