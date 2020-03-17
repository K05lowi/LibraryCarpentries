# NOTES ON UNIX LESSON


**Macbook pro:**
option + shift + 7 = /

option + shift + 8 = {

option + shift + 9 = }

option + shift + . = divide sign

control + f = logout

option + ¨ = ~

option + 9 = ]

option + 8 = [

option + 4 = £

option + y = \

option + i = | Note: copypaste pipe from fx wikepedia fx doesn't work on the commandline in Macbook pro



## IMPROVEMENTS

Set-up clarifications?

more examples - use cases. Think about how to use Shell in our library work and how to teach this practicality to our students. The
LC lessons are good for getting to understand the logic and concepts, but we need use cases. 

example using Nano/text editor

## CORRECTIONS

Correct mistake in exercise "working with free text" tr -d [:punct:] < 201403160_01_text.json > 201403160_01_text-nopunct.json

The correct file name is 000003160_01_text.json

Correct the following script: $ tr ' ' '\n' < 201403160_01_text-clean.txt | sort | uniq -c | sort -nr > 201403160_01_text-final.txt  replace the sort -nr with sort -r

## COMMENTS

GitBash runs fine - no need for warnings that it might not work. Just run GitBash 

In the "instructionals" download file can be better formulated with regards to setup instructions.

The didactical argument for using unix shell - when will students use it?
Why not Python or R from the very start?

The described approach is good (who you write and gather it together in input and output) is elegantly
described and this understanding is directly transferable to R and Python.

We cover alot of ground in the introductory exercises (variables, values, loops).

Perhaps more introduction to what is a variable and what is a value, what can they be used for, how are they remembered
in the system? Just in the current session or also the next time we open Shell.



