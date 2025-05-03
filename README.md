# 321-ComboMenu2

Complete the actvity based on the PLTW book.

#Include a video of the application working here.
def multiply_addition(a, b, c):
    return (a * b + c)

sandwich = input("What type of sandwich would you like? beef, tofu, chicken? ")
order = []
cost = 0.0

if sandwich == "chicken":
    number = int(input("How many? "))
    order.append("you ordered {number} chicken sandwich's")
    cost = multiply_addition(5.25, number, cost)
    
    
elif sandwich == "tofu":
    number = int(input("How many? "))
    order.append("you ordered {number} tofu sandwich's")
    cost = multiply_addition(5.75, number, cost)
  
   

elif sandwich == "beef":
    number = int(input("How many? "))
    order.append("you ordered {number} beef sandwich's")
    multiply_addition(6.00, number, cost)  
    



beverage = input("Would you like a beverage? (yes or no) ")

while beverage != "yes" and beverage != "no":
    print("Please enter 'yes' or 'no'")
    beverage = input("Would you like a beverage? (yes or no) ")

if beverage == "yes":
    size = input("What size beverage would you like? (small $1.00, medium $1.75, large $2.25) ")

    if size == "small":
        number = int(input("How many? "))
        order.append("you ordered {number} small beverages")
        cost = multiply_addition(1.00, number, cost)
        print("Your cost for this is", cost)

    elif size == "medium":
        number = int(input("How many? "))
        order.append("you ordered {number} medium beverages")
        cost = multiply_addition(1.75, number, cost)
        print("Your cost for this is", cost)

    elif size == "large":
        number = int(input("How many? "))
        order.append("you ordered {number} large beverages")
        cost = multiply_addition(2.25, number, cost)
        print("Your cost for this is", cost)

    else:
        print("Please either enter a beverage size or no")

elif beverage == "no":
    print("No beverage selected")
    
fries=input("would you like frech fries?")
while fries != "yes" and fries != "no":
    print("Please enter 'yes' or 'no'")
    fries = input("Would you like french fries? yes or no? ")

if fries == "yes":
    fsize = input("What size fries would you like? (small $1.00, medium $1.50, large $2.00) ")

    if fry_size == "small":
        mega = input("Would you like to mega-size your fries? yes or no? ")
        while mega != "yes" and mega != "no":
            print("Please enter 'yes' or 'no'")
            mega = input("Would you like to mega-size your fries? yes or no? ")

        if mega == "yes":
            number = int(input("How many? "))
            order.append("you ordered {number} large fries (mega-sized)")
            cost = multiply_addition(2.00, number, cost)
            
        elif mega == "no":
            number = int(input("How many? "))
            order.append("you ordered {number} small fries")
            cost = multiply_addition(1.00, number, cost)
            
    elif size == "medium":
        number = int(input("How many? "))
        order.append("you ordered {number} medium fries")
        cost = multiply_addition(1.50, number, cost)
        

    elif size == "large":
        number = int(input("How many? "))
        order.append("you ordered {number} large fries")
        cost = multiply_addition(2.00, number, cost)
        

    else:
        print("coose a valid size")

elif fries == "no":
    print("No fries selected")
    
ketchup=("Would you like any ketchup packs?")
if ketchup=='yes':
 number=int(input("How many?"))
 order.append("you ordered {number} large fries")
 cost = multiply_addition(0.25, number, cost)
if sandwich=="yes" and beverage=="yes" and fries=="yes":
  cost=cost-1
print("this is your total order", order )
print("your total cost is", cost)



