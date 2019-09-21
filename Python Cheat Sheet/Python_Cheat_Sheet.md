# Python 2

## Print to Screen
> print "Hello, World!"

Hello, World!

## Take User Input

> print('Enter your name:') <br>
> x = input()  # name: Mo Salah <br>
> print('Hello, ' + x)  <br>

Hello, Mo Salah


> Name = raw_input("what is your name? ") # input: Mo Salah <br>
> print(Name)

Mo Salah

> print "Enter a Sentence: " <br>
> print raw_input().replace(" ","-") <br>

Enter a Sentence: <br>
aa aa aa aa aa   <br>
aa-aa-aa-aa-aa   <br>


## Capitalize each Word in a String

> import string
>
> def solve(s):
>    words = s.split(" ")
>    for i in xrange(len(words)):
>      words[i] = string.capitalize(words[i])
>    
>    print " ".join(words)
>
> solve("hello world")


## Write List to File

> list = [5,6,7,8,9,10]
> with open('list_test.txt', 'w') as f:
>    for item in list:
>        f.write("%s\n" % item)

-------------------------------------------------------------------------------------------------------------------------------
# Python 3

## Print to Screen
> print("Hello, World!")

Hello, World!

## Take User Input

> Name = input("what is your name? ") # input: Mo Salah <br>
> print(Name)

Mo Salah

## Strip

>str = "Hello Hi ***" <br>
> print(str.strip(" * ")) <br>

Hello Hi

> a = "How are you?" <br>
> print(a) <br>
> a = a.split(" ")  <br>
> print(a) <br>

['How', 'are', 'you?']


> a = "-".join(a) <br>
> print(a)

How-are-you?



-----------
<pre>
SomeClass.py

class SomeClass:
    variable_1 = "This is a class variable"
    variable_2 = 100    #this is also a class variable.

    def __init__(self, param1, param2):
        self.instance_var1 = param1
        #instance_var1 is a instance variable
      	self.instance_var2 = param2   
        #instance_var2 is a instance variable
       
 main.py 
 
  from SomeClass import SomeClass
  obj1 = SomeClass("some thing", 18) 
  print obj1.variable_1                    # prints This is a class variable
  print obj1.instance_var1                 # prints some thing

https://medium.com/quick-code/understanding-self-in-python-a3704319e5f0
https://micropyramid.com/blog/understand-self-and-__init__-method-in-python-class/
</pre>
