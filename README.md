# Dictionary-of-Heights
This program asks the user for the heights of different people and creates a dictionary with the name of the person as the key and the value as the height

from fractions import Fraction
dictionary = {}
size = int(input("How many people do you wanna measure?: "))
for i in range(size):
    name = input("Enter the person's name: ")
    heightft = float(input("Enter the person's height (in ft): "))
    heightin = float(input("Enter the person's height (in in): "))
    height = ((heightft*12)+heightin)/12
    dictionary[name] = str(height) + " ft"
print(dictionary)
