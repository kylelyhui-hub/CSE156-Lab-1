CE156/CE157 LAB 1 (Oct 9/10)

You should use this lab to familiarise yourself with the Pycharm environment and work through some
examples from part 1 of the lecture slides.

Files stored on the C: drives in the lab machines will not persist (and you probably won’t be using the same
machine next time you are in a lab) so you need to save your work on your M: drive which is networked and
can be accessed from all University lab machines. On your M: drive create a folder for this module and
within this folder another new folder for the lab (e.g. M:\ce156\lab1).
Start Pycharm (you’ll find it under JetBrains on the Start menu). Select New Project and specify as the
location the folder you have just created.

We will initially be working in a Python console. Click on the Python Console icon (the top icon of those at
the bottom left of the window). In the console that appears you can try out fragments of Python code. Try
typing some simple expressions such as 67+135, 49-23, 7*29 and 17/3.

(Note that * is used for
multiplication in almost all programming languages.)

Now try 15/3, 17//3 and 15//3.

Observe that division using / always gives a real-number result even if the answer is an integer and that
division using // always truncates to a integer, ignoring any remainder.
Look at slides 13-20 in the lecture 1 slides; try out the examples on slide 14 and the exercises on slides 19-
21. Try to predict what the results will be before you see them. (In exercise 3 you should reset the value of x
to 8 after it has become 0.)

Now try typing the following expressions:

'hello ' + 'world'
'hi' * 3
5 * 'ho'
Now try
'hihihi' – 'hi'
'hihihi' / 3

Observe that errors are reported; we cannot subtract or divide strings.

We now wish to create scripts, or programs that we can save and resuse.

Right-click on the project name at the top of the left pane (i.e. lab1 if you used that name) and select New…
Python file. Supply a file name, e.g. program1.

You’ll now see a blank area in which you can type the script. When we run programs we need to control
precisely what’s output so we have to say explicitly what we want to print.

Type (or copy and paste) the following into the new blank area.
print('My first program')
name = input("What's your name? ")
print('Hello ', name)
print('6+7 is ', 6+7)

Run the program by right-clicking on the file name in the list pane and selecting the Run option.
The program will be run in a new area which is displayed where the console was previously seen. Note that
input is used to obtain input from the keyboard; the string in the parentheses will be displayed as a
prompt to the user asking for input. When you see the prompt type a name (followed by the return key).
print can be used to print an arbitrary number of items; by default it starts a new line and separates the
items using spaces.

When using input the keyboard input is stored as a string of characters; if we want it to be treated as a
number we need to explicitly convert it. 
Add the following lines to the end of your script

x = int(input("Enter value for x "))
y = int(input("Enter value for y "))
print('x+y is ', x+y)

Run the program again.

-------------------------------------------------------------------------------------------------------------------------
Exercise

Write a new script that asks the user to supply a number from the keyboard using int(input(…)), stores
the input value in a variable and outputs the square and cube of the number (with appropriate messages such
as “The square is”).

Work through the examples and exercises from part 1 of the lecture slides.

Also try some variations, such as a version of the circle exercise where the user is asked to supply the radius,
and a version of the currency-conversion exercise where the user is asked to supply the exchange rate and
the cost in dollars of three items in turn, outputting the equivalent cost in pounds and then calculating the
total and displaying it in both pounds and dollars.

To input an integer you need to use something like

 radius = int(input("Please enter the radius"))
 
and to input a real number you should use something like

 exchangeRate = float(input("Please enter the exchange rate"))
 
Run the programs with various different inputs, including some invalid ones, to observe what happens.
