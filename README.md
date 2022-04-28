
## About Me
My name is Thatcher Karsch. I am from a small town called Bonne Terre, Missouri. When I was younger, I wanted to be a genetic engineer after doing a project int the eighth grade. After going to college, I realized that is not what I wanted to do and started pursuing a career in the field of information technology. I have some prior experience from my early high school years and my military occupation also correlates to the IT field. I figured I would combine the two to further my knowledge and broaden the spectrum on which I was learning.

### Python

[![alt text](Coding.jpg)]

Python is a coding language I started learning when I was 14 years old. I stopped practicing it after about a year but have recently started picking it back up for my college coursework. Below you will see a program I wrote to calculate the total estimated cost to coat a cylinder in paint.

```markdown
import math
def get_nonnegative_float_from_user(prompt):
    while True:
        try:
            input_value = float(input(prompt))
            if (input_value < 0):
                print("Only nonnegative values are allowed. Please re-enter the value.")
                continue
            break
        except ValueError:
            print("Please enter a nonnegative numerical value.")
            continue
    return input_value
def perform_calculation():
        radius = get_nonnegative_float_from_user("Enter the cylinder's radius: ")
        height = get_nonnegative_float_from_user("Enter the cylinder's height: ")
        area = (2 * math.pi * radius * height + 2 * math.pi * radius **2)
        print ("The area of the cylinder is" ,area, "feet^2.")
        pints = (area / 5) 
        (math.ceil(pints)) 
        print ("There are" ,(math.floor(pints)), "pints required to coat the cylinder.") 
        cost = (pints * 8.75)
        (math.ceil (cost))
        print ("The total cost will be $" ,(round (cost, 2)))
def main():
        print("This program calculates the cost of coating a cylinder along with the area and the number of pints required.")
        while True:
                perform_calculation()
                response = input("Would you like to perform another calculation (y/n)? ")
                if (response == "y"):
                        print("")
                        continue
                else:
                        break
main ()
                
```
[Next](NationalGuard.md)
