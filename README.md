####Range (example:passing range into a function):####
The Python range() function is just a shortcut for generating a list, so you can use ranges in all the same places you can use lists.

range(6) # => [0,1,2,3,4,5]
range(1,6) # => [1,2,3,4,5]
range(1,6,3) # => [1,4]
The range function has three different versions:

range(stop)
range(start, stop)
range(start, stop, step)
In all cases, the range() function returns a list of numbers from start up to (but not including) stop. Each item increases by step.

If omitted, start defaults to zero and step defaults to one.

- **print ["O"] * 5**  
will print out ['O', 'O', 'O', 'O', 'O']

- **Create a 5 x 5 grid initialized to all 'O's and store it in board.**
board=[]
for x in range(0, 5):
    board.append(["O"]*5)


- **.join method**    
letters = ['a', 'b', 'c', 'd']
print " ".join(letters)
print "---".join(letters)
In the example above, we create a list called letters.
Then, we print a b c d. The .join method uses the string to combine the items in the list.
Finally, we print a---b---c---d. We are calling the .join function on the "---" string.

- **random number generator**  
from random import randint
coin = randint(0, 1)
dice = randint(1, 6)
In the above example, we first import the randint(low, high) function from the random module.
Then, we generate either zero or one and store it in coin.
Finally, we generate a number from one to six inclusive.

- **raw input**  
number = int(raw_input("Enter a number: "))
raw_input asks the user for input and returns it as a string. But we're going to want to use integers for our guesses! To do this, we'll wrap the raw_inputs with int()