Introduction
This project is about a scientific calculator that can solve linear and quadratic equations, store the equations and the solutions to the equations that have been previously performed so that the user can be able to access the calculations they performed previously and then graphically represent the 2D equations.
Application of Knowledge
(a)	To solve linear equations:
     Linear equations are in the form of ax+b=0. Here we are solving the equation to get the value of x.
First, I defined the function, I defined it as linear. This function does not take any parameter. The concept of writing my own functions in python, which is used here, is found on page 29 of the python book in chapter 1.
 Thus, the code allows the user to give the values of a, which is the coefficient of x, and b, which is the constant, using python’s input function. Since the input function gives a string, I had to use ‘eval’ to evaluate the string and get an integer which is what I wanted. The concept of Asking for input, which is used here, is found on page 99 of the python book in Chapter 3.
The linear equation ax+b=0 has a set of conditions, thus I had to use the selection statements in python. The concept of selection statements (if, else, elif), which is used here, is found on page 67 of the python book in chapter 2.  
If the value of the coefficient of x, which is a, is equal to zero, and  the value of the constant,   which is b, is not equal to zero, then the solution is undefined. The concept of relational operators and logical operators, which is used here, is found on page 65 of the python book in chapter 2.  Example: when b=5,
           0x+5=0, thus 0x=-5. Which means no value of x can give us -5, thus making the solution 
            Undefined.
   If the value of the coefficient of x, which is a, is equal to zero BUT the value of the constant, which is b, is also zero, then the solution has all real numbers. Example: when b=0,
0x+0=0, thus 0x=0. Which means x can be any real number, then the solution to the             equation is all real numbers.
When the user inputs the coefficient of x, which is a and the value is not equal to zero, then the code performs the math which is x is = (-b/a).  The concept of which division sign I will use to get a floating point number, which is used here, is found on page 13 in chapter 1. 
Since I want the user to be able to access the calculation they previously performed, thus my code should open, append and read the calculations from a text file. Therefore, I created a variable f to open the file named ‘linearfile.txt’. Open takes 2 arguments, the name of the file we intend to open and the string that represents the kind of operation we want to perform on the file. As for my code it took ‘linearfile.txt’ and ‘a+’ for append and plus sign meaning if it is not there create it. Then using the write function to enter data into the file, the output I want to display on my file is ‘The solution for (the linear equation you want), is x= (then the value of x we got)’ Here I used the concept of  string concatenation, to put the strings and the integers (as str x) one after another, this is found on page 85 in chapter 3 of the python book.. Then f.close to close the file. This was to store the calculations they perform. After that the code then returns the value of x. Moreover, if the user want to access their previous calculations, my code has a function defined as history. Which is the code to read the file. Therefore, I created a variable f to open the file named ‘linearfile.txt’. Open takes 2 arguments, the name of the file we intend to open and the string that represents the kind of operation we want to perform on the file. As for my code it took ‘linearfile.txt’ and ‘r’ for the read mode. I then use the mode function to check that the file is in open mode and if it is, then I proceed ahead. I use f.read mode to read the file and print its contents. I then used the while loop to read from the file that contains the equations and their solutions. This concept of writing a file, opening, closing and reading it, which is used here, is found on page 156-164 of the python book in chapter 5.  The concept of Appending, which is used here, is found on page 125 in chapter 4. This concept of while loop is found on page 173 of the python book in chapter 5. 
(b)	To solve quadratic equations.
  Here I had to import the math module first as it does not come with python by default.
Quadratic equations are in the form of  ax^2+bx+c=0. Here we are solving the equation to get the values of x_1 and x_2.
First, I defined the function, I defined it as quadratic. This function does not take any parameter. The concept of writing my own functions in python, which is used here, is found on page 29 of the python book in chapter 1.
 Thus, the code allows the user to give the values of a, which is the coefficient of x^2, then b, which is the coefficient of x, and c, which is a constant, using python’s input function. Since the input function gives a string, I had to use ‘eval’ to evaluate the the string and get an integer which is what I wanted. The concept of Asking for input, which is used here, is found on page 99 of the python book in Chapter 3.
The quadratic equation ax^2+bx+c=0 has a set of conditions, thus I had to use the selection statements in python. The concept of  selection statements (if, else, elif), which is used here, is found on page 67 of the python book in chapter 2. 
     If the value of the coefficient of x^2, which is a, is equal to zero, also the value of the coefficient of x, which is b, is equal to zero, and the value of the constant, which is c is also zero. Then the solution is ‘undetermined’. Example; when a=0, b=0, c=0
    0x^2+0x+0=0, then all real numbers can be used thus making the solution ‘undetermined’.
      Although if the value of the coefficient of x^2, which is a, is equal to zero, also the value of the coefficient of x, which is b, is equal to zero, and, the value of the constant, which is c is not equal to zero. Then there is ‘no solution’. Example; when a=0, b=0, c=5
         0x^2+0x+5=0, then it will be 0x^2+0x=-5, no value of x can be used to get -5, thus I say ‘no solution’.
    Then there are times that the value of the coefficient of x^2, which is a, is equal to zero,  but the value of the coefficient of x, which is b, is not equal to zero. Then the equation turns to be linear and so we solve for x, (-c/b). Example; when a=0, b=4, c=3
        0x^2+4x=-3.
Else, if the value of a is not equal to zero, then we have a delta which is b**2 - 4*a*c, then I find the square root of the delta, but first I have to check whether delta is equal to or greater than zero, as you cannot get the square root of a negative number. So if it is greater than zero or equal to zero so I go on and find the square root, here I use the math module I imported.
I then store the two values of x in a list. This is a concept on lists found on page 120 in chapter 4 of the python book.
Since I want the user to be able to access the calculation they previously performed, thus my code should open, append and read the calculations from a text file. Thus, I Repeat the procedure I used on linear equation of writing, opening, appending and reading a file.
(c). To graphically represent the 2D equations.
Here I had to import the Turtle module and the Random module first, as they do not come with python by default.
The concept of using the Turtle module is found on page 24 in chapter 1 of the python book.
 I then define the function, called graph. This function graphs the equation of the form a*x+b*y+c=0, thus it takes a, b and the constant c as parameters. The concept of writing my own functions in python, which is used here, is found on page 29 of the python book in chapter 1.
I'm using randomization to get a value of x which will help me to solve and get the value of y, and thus get a point. using two points I can draw the line.
However, randomization of x has a certain range to prevent the line being tiny.
I then use the for loop to draw the x-axis and the y-axis grid. This concept of ‘for loop’ is found on page 33 in chapter 1 of the python book.
For me to draw the graph of the 2D equations, I need two points. So I stored the points in a dictionary, one dictionary called points_1, which took ‘x’ as the key and the value of x_1 after randomization as the value, I did the same case to the second dictionary.  This is concept of dictionaries is found on page 135 in chapter 4.
I then use the ‘goto’ function in turtle module which takes the values from the dictionary as the argument. I then draw the line of the given equation.


  
       				References.
Miller, B. N., & Ranum, D. L. (2014). Python programming in context. Jones & Bartlett   
Publishers.
