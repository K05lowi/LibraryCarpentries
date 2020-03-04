#Regular Expressions
##Formulation of lessons
The formulation of some of the questions can be improved. This could be our contribution to improving the LC lessons.

###Examples for improvement of formulation
Erik's example: How would you match the date format dd-MM-yyyy or dd-MM-yy at the end of a line only?
The formulation indicates that we have to find dates that end with four digits in the year or 2 digits. However the suggested
solution also findes years with 3 digits, which is useful if you want to find mistakes in the data but does not answer the question.
The solution is this: \d{2}-\d{2}-\d{2,4}$
Erik's solution uses the "OR" expression: \d{2}-\d{2}-\d{2}$|\d{2}-\d{2}-\d{4}$



##Aditional exercises in the RegEx lesson
*1 To the lesson "extracting a substring in Google Sheets using regex, a nice addition would be guidance how to move an entire 
column of information instead of just one cell at a time. Thanks to Ene, we have the following expression

=ArrayFormula (if(len(G2:G),REGEXEXTRACT(G2:G,"\d+\.\d+, -?\d+\.\d+")

It is necessary to use an **if len** to set parameters \(tell the computer where to put the data)\.
Make sure the parenthesis encaspulate the expression correctly

*2 A general exercise in looking for patterns in a string, that man later can use in the expressions.
