<!DOCTYPE html>
<html>
  <head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
  </head>
<body>
    <h2>About Me</h2>
           <p> My name is Thatcher Karsch. I am from a small town called Bonne Terre, Missouri. When I was younger, I wanted to be a genetic engineer after doing a project int the eighth grade. After going to college, I realized that is not what I wanted to do and started pursuing a career in the field of information technology. I have some prior experience from my early high school years and my military occupation also correlates to the IT field. I figured I would combine the two to further my knowledge and broaden the spectrum on which I was learning. </p>

 
<h3>Python</h3>
   <img src="Coding.jpg"> 
            <p> Python is a coding language I started learning when I was 14 years old. I stopped practicing it after about a year but have recently started picking it back up for my college coursework. Below you will see a program I wrote to calculate the total estimated cost to coat a cylinder in paint. </p>

<code>
import math<br>
def get_nonnegative_float_from_user(prompt):<br>
    while True:<br>
        try:<br>
            input_value = float(input(prompt))<br>
            if (input_value < 0):<br>
                print("Only nonnegative values are allowed. Please re-enter the value.")<br>
                continue<br>
            break<br>
        except ValueError:<br>
            print("Please enter a nonnegative numerical value.")<br>
            continue<br>
    return input_value<br>
def perform_calculation():<br>
        radius = get_nonnegative_float_from_user("Enter the cylinder's radius: ")<br>
        height = get_nonnegative_float_from_user("Enter the cylinder's height: ")<br>
        area = (2 * math.pi * radius * height + 2 * math.pi * radius **2)<br>
        print ("The area of the cylinder is" ,area, "feet^2.")<br>
        pints = (area / 5) <br>
        (math.ceil(pints)) <br>
        print ("There are" ,(math.floor(pints)), "pints required to coat the cylinder.") <br>
        cost = (pints * 8.75)<br>
        (math.ceil (cost))<br>
        print ("The total cost will be $" ,(round (cost, 2)))<br>
def main():<br>
        print("This program calculates the cost of coating a cylinder along with the area and the number of pints required.")<br>
        while True:<br>
                perform_calculation()<br>
                response = input("Would you like to perform another calculation (y/n)? ")<br>
                if (response == "y"):<br>
                        print("")<br>
                        continue<br>
                else:<br>
                        break<br>
main ()
                
</code>
</body>
</html>
[Next](NationalGuard.md)
