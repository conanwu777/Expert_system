# Expert_system
A backwards chaining inference engine which evaluates quires through logical deduction from known facts

In artificial intelligence, an expert system is a computer system that emulates the decision-making ability of a human expert. Expert systems are designed to solve complex problems by reasoning through bodies of knowledge, represented mainly as if–then rules rather than through conventional procedural code. The first expert systems were created in the 1970s and then proliferated in the 1980s. Expert systems were among the first truly successful forms of artificial intelligence (AI) software.
(visit https://en.wikipedia.org/wiki/Expert_system to read more)

This project is done in collaboration with Liam Dehaudt, we implemented a simple infrenence engine using backwards chaining which is able to reason through given facts and deductions to derive conclusion about the quires.

## Compiling and running
Run `make`. An executable will compile. Currently only tested on OS X.

Run with `./expert_system "fact_file"`. A few sample knowledge base files can be found in the root, named `test`, `test2` and `test3`

To construct new knowledge base files, see:
![alt text](/1.png)


## Features

* Handles AND(+), OR(|), NOT(!) and XOR(^) operators in both assertion and conclusion

* Handles nested parenthesized expressions

* Handles biconditional rules IFF (<=>)

* Stores knowledge in a global graph of fact nodes linked by rules to minimize repeated computation

* Interactive fact validation to fiddle with the input while running (can update both facts and quires in runtime)

* Complete deduction reasoning outputted in one-liner formal logic notation directly from base facts

* 4 levels of truth in terms of confidence in deduction

  - surely TRUE (rely only on known fact without any further assumption)
  
  - TRUE assuming some unspecified (and un-deductible) variables being defaulted to false
  
  - FALSE assuming some unspecified (and un-deductible) variables being defaulted to false
  
  - surely FALSE (rely only on known fact without any further assumption)
  
## Sample screenshots:
![alt text](/2.jpg)
