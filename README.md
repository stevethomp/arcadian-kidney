# Simple RPN Calculator
This is a basic technical qualifier test.
Candidates should fork the repo and implement the specifications below on the assigned platform. The candidate's repo will be used for evaluation.

# Reverse Polish Notation
In reverse Polish notation the operators follow their operands; for instance, to add 3 and 4, one would write "3 4 +" rather than "3 + 4". If there are multiple operations, the operator is given immediately after its second operand; so the expression written "3 − 4 + 5" in conventional notation would be written "3 4 − 5 +" in RPN: 4 is first subtracted from 3, then 5 added to it. An advantage of RPN is that it removes the need for parentheses that are required by infix. While "3 − 4 × 5" can also be written "3 − (4 × 5)", that means something quite different from "(3 − 4) × 5". In postfix, the former could be written "3 4 5 × −", which unambiguously means "3 (4 5 ×) −" which reduces to "3 20 −"; the latter could be written "3 4 − 5 ×" (or 5 3 4 − ×, if keeping similar formatting), which unambiguously means "(3 4 −) 5 ×".

Despite the name, reverse Polish notation is not exactly the reverse of Polish notation, for the operands of non-commutative operations are still written in the conventional order (e.g. "÷ 6 3" in Polish notation and "6 3 ÷" in reverse Polish both evaluate to 2, whereas "3 6 ÷" in reverse Polish notation would evaluate to ½).

# Notes
* For the purposes of this evaluation, function comes before form. Don't get so busy with looks that you miss the required functionality. Leave fonts, colors, and pixel pushing until you've satisfied all the functional requirements.
* Be sure to read the 'Requirements' below and implement each as stated.
* If a requirement is unclear, make a reasonable assumption and clearly state this assumption in the 'Assumptions' section immediately below.

# Assumptions
* None

# Layout
![RPN Layout](rpn_layout.png?raw=true "Layout")

# Requirements
* Layout as pictured above
* Color display portion as shown (Black text on Green background)
* Clear _(C)_ button Erases memory. Back to start.
* Reversed Polish Notation number entry

# Input Examples
Number _(Button)_ --> Result
* _(C)_ --> 0
* 6, _(Enter)_, 4, _(+)_ --> 10
* 6, _(Enter)_, 6, _(Enter)_, 3, _(Enter)_, 2, _(‐)_, _(+)_, _(*)_ --> 42
* 1, _(Enter)_, 5, _(/)_ --> 0.2
* 1, _(+)_ --> Error
* 5, _(Enter)_, _(/)_ --> Error
* 5, _(Enter)_, 4, _(Enter)_, _(‐)_, _(*)_ --> Error
* _(Enter)_	--> No change

# Bonus (in order of importance)
* Divide up your work into tasks. Each commit corresponds to a task.
* Use Github's issue tracker to record your tasks, bugs, improvements, etc.
* Implement the _Input Examples_ above as unit tests
* Reference the issue tracker task in commit message
* Make it pretty
* Add more unit tests
