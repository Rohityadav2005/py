# Exercise: Functions in python
1. Write a function called calculate_area that takes base and height as an input and returns and area of a triangle. Equation of an area of a triangle is,

area = (1/2)*base*height
def calculate_area(base,height):
    area = 1/2 * base * height
    return area

base = int(input("enter the base of the triangle \n"))
height = int(input("enter the height of the triangle \n"))
calculate_area(base,height)

print("the area of the triangle",calculate_area(base,height))

2. Modify above function to take third parameter shape type. It can be either "triangle" or "rectangle". Based on shape type it will calculate area. Equation of rectangle's area is,
```
rectangle area=length*width
```
If no shape is supplied then it should take triangle as a default shape

def tri_area_cal(tri_base,tri_height):
    tri_area = 1/2 * tri_base * tri_height
    return tri_area

def rect_area_cal(rect_height,rect_width):
    rect_area = rect_height * rect_width
    return rect_area


shape = input("enter the shape \n")
if(shape=="Rectangle"):
    rect_height = int(input("enter the height of the rectangle \n"))
    rect_width = int(input("enter the height of the rectangle \n"))
    print("The area of the rectangle is :",rect_area_cal(rect_height,rect_width))
else :
    tri_base = int(input("enter the base of triangle \n"))
    tri_height = int(input("enter the height of the triangle \n"))
    print("The area of the triangle is:",tri_area_cal(tri_base,tri_height))


3. Write a function called print_pattern that takes integer number as an argument and prints following pattern if input number is 3,
```
*
**
***
```
if input is 4 then it should print
```
*
**
***
****
```
def pat(n):
    for i in range(1,n+1):
        print("*" * i)

n = int(input("enter the number of line for pattern you want \n"))
pat(n)

Basically number of lines it prints is equal to that number. (Hint: you need to use two for loops)

[Solution](https://github.com/codebasics/py/blob/master/Basics/Exercise/10_functions/10_functions_exercise.py)
