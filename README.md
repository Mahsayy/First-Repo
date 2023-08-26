# Basics of Python
#1-This is a comment ================================================================================
print("Hello Word!")

#2-How to make variable ==============================================================================
age = 20
sentence = "My name is Mahsa"
print (age)
print (sentence)

#3-to assign number to each variable ==================================================================
sarah,bob,mike = 13, 72, 12
print (sarah)

#4-to assign only one number to all ===================================================================
Ali = Mahyar = Amir =20
print (Ali)

#5-print more than one thing ==========================================================================
name , age = "Mahsa" , 27
print (name,age)

#6-Arithmetic operators ===============================================================================
# + - * / %
age1 = 5
age2 = 6
print (age1 + age2)
print(age1 * age2)
print (age1 / age2)
print (age1 % age2)
print (age1 - age2)

#7- combining two strings ============================================================================
first_name = "Mahsa"
last_name = "Younesi"
print (first_name + " " + last_name) #we add " " to add a space between tow variables 

#8- print idexes from a string ========================================================================
sent3 = "Mahsa is beautiful" 
print (sent3[0:4]) #starts from 0 and ':' means 'to'

#9- Placeholders in Strings ===========================================================================
#9-1 %s %d --------------------------------------------------------------------------------------------
name = "jake"
print (name + " " + "is 15 years old") #name is a placeholder here
#BUT INSTEAD WE CAN USE PLACEHOLDERS
name = "Ali"
sentence = "%s is 15 years old" # %s is for string and %d is for integer
print(sentence % name)

sent4 = "%s %s is the best guy in the world"
print (sent4 %("mahsa" , "younesi")) #for more than one, we should add parenthesis after %

sent5 = " %s is %d years old"
print(sent5 % ("Mahi", 23)) 

#9-2 Format strings -----------------------------------------------------------------------------------
#f"{}"
name = "avi"
print (f"my name is {name} .")
age = 12
print (f"my age is {age}.")

#EXERCISE 1 ==============================================================================================
#1
sum = (15 + 30)/2
print (sum)

#2
a = 10
b = 25
add = a + b
sub = a - b
div = a/b
bagh = b%a
mult = a*b
print (add," ",sub, " ", div, " ", bagh, " ", mult)

#3
name = "Mahsa"

#4
Mahsa, Abbas , Mahyar = "Lasagna" , "Loobia polo" , "Pizza"
print (Mahsa, Abbas, Mahyar)

#5
print (("Hello!" + " ") * 10)

#6 
name , age = "Mahsa" , 27
print (name, age)

#7
name = "Abbas"
age = "twenty nine"
who = name + age

#8
name = "abolghasem"
print (name[3])

#9
job = "firefighter"
print (job[0:5])

#10
surname = "amiritaeme"
print (surname[0:])
#============================================================================================================

#10- List ===================================================================================================
#what is list? ordered items, have an index, has an order

shopping_list = ["apples","bananas" ,"oranges" ,"tape" ,"scissor" ,"wrapping paper" ]
#note that index starts from 0, index 0 here is apple (arayeh)
print(shopping_list)
print(shopping_list[0:2])
print(shopping_list[0])

#10-1 ADD item to your list using .append() ---------------------------------------------------------------------
shopping_list.append("blue berries")

#10-2 CHANGE item in list --------------------------------------------------------------------------------------
shopping_list [0] = "cherries"
print(shopping_list)

#10-3 DELETE items using del ------------------------------------------------------------------------------------
del shopping_list[2]
print(shopping_list)

#10-4 lenght of list using len() ---------------------------------------------------------------------------------
print (len(shopping_list))

#10-5 Combine to lists using +  ----------------------------------------------------------------------------------
shopping_list2 = ["battery" , "laptop" , "tea bag"]
print (shopping_list + shopping_list2)
 #you can also use * / - % as well as in the list

#10-6 Max & min in a list of numbers ----------------------------------------------------------------------------
age = [2,1,5,9,6,7,2,0,4]
print(max(age))
print(min(age))

#11- Dictionary ===================================================================================================
#for dictionary we have key and a corresponadant value dictionary is made using { : }
students = {"Mahsa":27 , "Mahyar": 20 , "Abbas":29}
print (students)
print (students["Mahsa"])

#11-1 UPDATE a value in dictionary ---------------------------------------------------------------------------------
students["Mahsa"] = 28
print (students)

#11-2- DELETE a value from dictionary using del --------------------------------------------------------------------------
del students["Abbas"]
print (students)

#11-3- Count the number of elements is a dictionary using len ------------------------------------------------------------
print(len (students))

#12- Tuples using ( , , ) ==================================================================================================
#Tuples can be modified / safety / consistency
tup = ("pilot" , "firefighter" , "teacher")
#u can not delete or add an index in tuple like list or dictionary, if you do, you'll face error
print (tup[0])
print (tup[0:])

#12-1- make new tuple using + ----------------------------------------------------------------------------------------------
tup = ("pilot" , "firefighter" , "teacher")
tup2 = (12 , 13, 15 , 68)
tup3 = tup + tup2
print (tup3)

#13- Conditional Statements if else =======================================================================================
if 3<2:
    print("Hello")
else:
    print("comdition was not true")

#realtional operators
#< > <= >= == !=

#13-3 elif (else if) --------------------------------------------------------------------------------------------------------
age = 19
if age<15:
    print ("you are younger than 15")
elif age == 16: 
    print ("you are 16")
elif age == 17:
    print ("you are17")
else:
    print ("you are older than 16") 
   
#and / or
#you can use 'and' to rwquire both condition is true
# 'or' just one of them is true, the condition is true

#14 for Loops ===================================================================================================================
list1 = ["apples" , "bananas"  , "grapes"]
tup1 = (1,6,12)
for item in list1:
    print (item)
for item in tup1:
    print (item)

#14-1- range function ----------------------------------------------------------------------------------------------------------
for i in range(1,11):
    print (i)

for item in range(0,10):
    print (item)

#14-2 increment factor --------------------------------------------------------------------------------------------------------
for i in range (0,15,2): #number 2 here is added to the current number to get the next number
    print (i)

#14-3 nest a for loop in another for loop ------------------------------------------------------------------------------------
for i in range (0,5):
    for j in range (0,3):
        print (i*j)


#15-
