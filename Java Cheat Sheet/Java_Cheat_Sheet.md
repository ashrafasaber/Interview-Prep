# Java

## Arrays

## TreeMaps

## HashMaps

## Stack

## Queue

## if-then
 
## Switch
> switch(expression) { <br>
>  case x: <br>
>    // code block <br>
>    break; <br>
>  case y: <br>
>    // code block <br>
>    break; <br>
>  default: <br>
>    // code block <br>
> } <br>



> int day = 4; <br>
> switch (day) { <br>
>  case 1: <br>
>    System.out.println("Monday"); <br>
>    break; <br>
>  case 2: <br>
>    System.out.println("Tuesday"); <br>
>    break; <br>
>  case 3: <br>
>    System.out.println("Wednesday"); <br>
>    break; <br>
>  case 4: <br>
>    System.out.println("Thursday"); <br>
>    break; <br>
>  case 5: <br>
>    System.out.println("Friday"); <br>
>    break; <br>
>  case 6: <br>
>    System.out.println("Saturday"); <br>
>    break; <br>
>  case 7: <br>
>    System.out.println("Sunday"); <br>
>    break; <br>
> } <br>
> // Outputs "Thursday" (day 4) <br>

## While

> while (condition) { <br>
>  // code block to be executed <br>
> } <br>

> int i = 0; <br>
> while (i < 5) {  <br>
>  System.out.println(i); <br>
>  i++; <br>
> }<br>

## Do-While

> do {   <br>
>   // code block to be executed <br>
> } <br>
> while (condition); <br>

> int i = 0; <br>
> do {<br>
>  System.out.println(i);<br>
>  i++;<br>
> } <br>
> while (i < 5);<br>

## For
> for (int i = 0; i < 5; i++) {  <br>
>  System.out.println(i); <br>
> } <br>

> for (type variable : arrayname) { <br>
>  // code block to be executed <br>
> } <br>

> String[] cars = {"Volvo", "BMW", "Ford", "Mazda"}; <br>
> for (String i : cars) { <br>
>  System.out.println(i); <br>
> } <br>
## Constructors
------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------
## Primitives

1-boolean  <br>
2-byte <br>
3-short <br>
4-int <br>
5-long <br>
6-float <br>
7-double <br>
8-char <br>

Primitive types hold their values in memory
You can call methods on references but not primitives
------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------

## Reference Types
Refers to an object
------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------
## String

> String reference = "Good Morning"; <br>
> int len = reference.length();  // calling method on reference <br>


> String name = "Fluffy"; <br>
> String name = new String("Fluffy"); <br>
------------------------------------------------------------------------------------------
### length()

> String a = "abcdefghijklmnopqrstuvwxys" <br>
> System.out.println(a.length()); <br>
------------------------------------------------------------------------------------------

### charAt()
>String a = "abcdefghijklmnopqrstuvwxys"  <br>
>System.out.println(a.charAt(0));<br>
>System.out.println(a.charAt(1));<br>
>System.out.println(a.charAt(2));<br>
------------------------------------------------------------------------------------------

### indexOf()
snippet from OCA book

>int indexOd(int ch) <br>
>int indexOf(char ch, int fromIndex) <br>
>int indexOf(String str) <br>
>int indexOf(String str, index fromIndex) <br>


> String string = "animals"; <br>
> System.out.println(a.indexOf('a'));		// 0  <br>
> System.out.println(a.indexOf('al'));		// 4 <br>
> System.out.println(a.indexOf('a',4));		// 4 <br>
> System.out.println(a.indexOf('al',5));		// -1  if -1 this means no match found <br>

------------------------------------------------------------------------------------------
### substring()
> string substring(int beginIndex) <br>
> string substring(int beginIndex, int endIndex) <br>

String string = "animals";<br>
a  n  i  m  a  l  s<br>
0  1  2  3  4  5  6<br>

> System.out.println(a.substring(3));			 // mals <br>
> System.out.println(a.substring(string.indexOf('m')));	 // mals <br>
> System.out.println(a.substring(3, 4));			 // m <br>
> System.out.println(a.substring(3, 7));			 // mals <br>

> System.out.println(a.substring(3, 3));			 // empty string <br>
> System.out.println(a.substring(3, 2));			 // throws exception <br>
> System.out.println(a.substring(3, 8));			 // throws exception <br>

------------------------------------------------------------------------------------------
### toLowerCase() and toUpperCase()
                               
> String toLowerCase() <br>
> String toUpperCase() <br>

> String string = "animals"; <br>
> System.out.println(string.toUpperCase());       // ANIMALS <br>
> System.out.println("Abc123".toLowerCase());     // abc123 <br>
------------------------------------------------------------------------------------------
### equals() and equalsIgnoreCase()

> boolean equals(Object obj) <br>
> boolean equalsIgnoreCase(String str) <br>

> System.out.println("abc".equals("ABC"));	     //  false	<br>
> System.out.println("ABC".equals("ABC"));	     //  true <br>
> System.out.println("abc".equalsIgnoreCase("ABC"));   //  true <br>

------------------------------------------------------------------------------------------
### startsWith() and endsWith()

> boolean startsWith(String prefix) <br>
> boolean endsWith(String suffix) <br>

> System.out.println("abc".startsWith("a"));	//  true <br>
> System.out.println("abc".startsWith("A"));	//  false <br>
> System.out.println("abc".endsWith("c"));	//  true <br>
> System.out.println("abc".endsWith("a"));	//  false <br>

------------------------------------------------------------------------------------------
### contains()

> boolean contains(String str) <br>

> System.out.println("abc".contains("b")); // true <br>
> System.out.println("abc".contains("B")); // false <br>
------------------------------------------------------------------------------------------
### replace()

> String replace(char oldChar, char newChar); // AbcAbc <br>
> String replace(CharSequence oldChar, CharSequence newChar) <br>

> System.out.println("abcabc".replace('a', 'A'));  // AbcAbc <br>
> System.out.println("abcabc".replace("a","A"));   // AbcAbc  <br>

------------------------------------------------------------------------------------------
### trim()

> public String trim() <br>

> System.out.println("abc".trim());  // abc <br>
> System.out.println("\t a b c \n".trim());  // a b c  <br>
------------------------------------------------------------------------------------------
### Method Chaining



------------------------------------------------------------------------------------------          
------------------------------------------------------------------------------------------

## StringBuilder

------------------------------------------------------------------------------------------
## StringBuffer

------------------------------------------------------------------------------------------
## ArrayList


------------------------------------------------------------------------------------------                             
## Functions

------------------------------------------------------------------------------------------                             
## Big O

http://bigocheatsheet.com/


------------------------------------------------------------------------------------------
## Searching

------------------------------------------------------------------------------------------
## Sorting

------------------------------------------------------------------------------------------
## 

> Student ashraf = new Student();

------------------------------------------------------------------------------------------
##

##

##
