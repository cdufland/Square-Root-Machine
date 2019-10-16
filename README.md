# Square-Root-Machine
"This program allows the user to calculate the square root of a method based on two different methods. 
It also generates the square root based on the Math.sqrt method in Java to compare the two answers. 
To use the program the user enters a number (that is greater than zero but less than One billion) for 
which they want to find the square root. They can then enter how accurate they would like that result 
to be using the given method. They can go from 0 to 15 decimal places. The user selects a method and 
then presses the calculate button. At that point the program first calculates a seed value. This value 
represents a first guess to start calculations. The seed value is calculated by first taking the log 
base ten of the user provided number. That number is then divided by two and stored as an integer
(a whole number) it is then multiplied by two to get an even number exponent. At that point the number 
is then divided by 10 raised to the even number exponent. This gets the base value which is compared to
10 if its greater or equal the seed value will be of the form (6*(10^n)) power where n is the even number
exponent previously calculated divided by 2. If that number is less than 10 then the seed value will take
the form 2*10^n where n is the is the even number exponent previously calculated divided by 2. Once the 
seed value is calculated the program then calculates the square root based on the method specified by the
user. For the Newton Method the following formula is used x1 = ( x0 + ( numbe r/ x0 ) ) / 2) where 
x1= the next guess to be compared to the actual square root x0= the previous guess \nnumber = the user 
inputted number this process is repeated with x1 becoming x0 and a new guess being calculated in later 
iterations, until x1 is suitably close to the actual square root.\n\nFor the Bakhshali method  the 
following formulas are used aN = ( number- x0^2)/ ( 2 * x0)\nbN = x0 + aN x1 = bN - ( aN^2 / ( 2x0 + aN)) 
where aN= represents a first guess bN = the original guess plus this first guess x1 represents the 
final guess to be compared to the actual square root. This method essentially has two guesses built into
one iteration.This process repeats until it is suitably close to the actual square root, it repeats at least
five times.The program then uses the estimated value to calcule an error which is as follows 
|actual-estimate|/actual * 100 actual = the actual square root of the number estimate = the square root
calculated based on the chosen method\nit then outputs as a percentage. The number of iterations that 
needed to be conducted to get suitably close to the actual square root appear below the error.
https://en.wikipedia.org/wiki/Methods_of_computing_square_roots 
This program is for educational purposes only.
