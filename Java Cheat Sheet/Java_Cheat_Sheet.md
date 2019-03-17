# Java

## Arrays

## TreeMaps

## HashMaps

## Stack

## Queue

## if-then
 
## Switch

## While

## Do-While

## For

## Constructors
------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------
## Primitives

1-boolean
2-byte
3-short
4-int
5-long
6-float
7-double
8-char

Primitive types hold their values in memory
You can call methods on references but not primitives
------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------

## Reference Types
Refers to an object
------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------
## String

String reference = "Good Morning";
int len = reference.length();  // calling method on reference


String name = "Fluffy";
String name = new String("Fluffy");
------------------------------------------------------------------------------------------
### length()

String a = "abcdefghijklmnopqrstuvwxys"
System.out.println(a.length());
------------------------------------------------------------------------------------------

### charAt()
String a = "abcdefghijklmnopqrstuvwxys"
System.out.println(a.charAt(0));
System.out.println(a.charAt(1));
System.out.println(a.charAt(2));
------------------------------------------------------------------------------------------

### indexOf()
snippet from OCA book

int indexOd(int ch)
int indexOf(char ch, int fromIndex)
int indexOf(String str)
int indexOf(String str, index fromIndex)


String string = "animals";
System.out.println(a.indexOf('a'));		// 0
System.out.println(a.indexOf('al'));		// 4
System.out.println(a.indexOf('a',4));		// 4
System.out.println(a.indexOf('al',5));		// -1  if -1 this means no match found

------------------------------------------------------------------------------------------
### substring()
string substring(int beginIndex)
string substring(int beginIndex, int endIndex)

String string = "animals";
a  n  i  m  a  l  s
0  1  2  3  4  5  6

System.out.println(a.substring(3));			 // mals
System.out.println(a.substring(string.indexOf('m')));	 // mals
System.out.println(a.substring(3, 4));			 // m
System.out.println(a.substring(3, 7));			 // mals

System.out.println(a.substring(3, 3));			 // empty string
System.out.println(a.substring(3, 2));			 // throws exception
System.out.println(a.substring(3, 8));			 // throws exception

------------------------------------------------------------------------------------------
### toLowerCase() and toUpperCase()
                               
String toLowerCase()
String toUpperCase()

String string = "animals";
System.out.println(string.toUpperCase());       // ANIMALS
System.out.println("Abc123".toLowerCase());     // abc123
------------------------------------------------------------------------------------------
### equals() and equalsIgnoreCase()

boolean equals(Object obj)
boolean equalsIgnoreCase(String str)

System.out.println("abc".equals("ABC"));	     //  false	
System.out.println("ABC".equals("ABC"));	     //  true
System.out.println("abc".equalsIgnoreCase("ABC"));   //  true

------------------------------------------------------------------------------------------
### startsWith() and endsWith()

boolean startsWith(String prefix)
boolean endsWith(String suffix)

System.out.println("abc".startsWith("a"));	//  true
System.out.println("abc".startsWith("A"));	//  false
System.out.println("abc".endsWith("c"));	//  true
System.out.println("abc".endsWith("a"));	//  false

------------------------------------------------------------------------------------------
### contains()


boolean contains(String str)

System.out.println("abc".contains("b")); // true
System.out.println("abc".contains("B")); // false
------------------------------------------------------------------------------------------
### replace()


------------------------------------------------------------------------------------------
### trim()


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
## Searching

------------------------------------------------------------------------------------------
## Sorting

------------------------------------------------------------------------------------------
## 

Student ashraf = new Student();

------------------------------------------------------------------------------------------
##

##

##