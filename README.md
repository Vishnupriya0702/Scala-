# Scala-
Scala supports functional as well as Object oriented programming languages.
Everything is object in scala, including functions.
Declaring variables in Scala :
Varibales can be declared through 2 sets: val, var. val means immuatble variable, var means mutable variable.

Example : val x: Int =10;
So, 10 is immutable value

var x: Int =10;
10 is mutable and it can be changed.

Type Inference is supported in scala.

Expression and blocks:
all the expressions can be written in a line like below :
val x = { val a=10; val b=20; a+b}

Lazy evaluation: Main feature which is used in Spark:
while declaring variables, we can assign like below :
lazy val x=100;
Int <lazy>
  
Lazy evaluation is same as DAG in Spark.

foreach(printlin) - iterative statement in scala.

For Loop:
for(i<-arguments) code
for ( i<- 5 to 1 by -2) println(i)

For Loop with Guard condition:
Assigning for loop with if condition, so only if condition is passed it goes to the next println statement, else it would be running the loop.

For Instance :
for(i<- 1 to 5; j<- 1 to 4) {
     if(i==j)
     println(s "($i, $j)"}
     
 In the above loop, it process all the records in for loop and then go inside the bracket condition.
 
 But, if we change the for loop like the below one:
 for(i<- 1 to 5; j<- 1 to 4, if i==j) {
   println(s "($i, $j)"}
   
In the above loop, once the record is processed , it checks for the if condition, if no match s there, it goes into the loop again, which improves the performance.

yield is a keyword to collect for for loop(in iterative). It is applied only in for loop.

Function in Scala:
  def function_name(function_params): return_type ={
  code
  }
  def areaRect(1:Float, b: Float): Float={
  l*b
  }
  
  def isEven_number(i : int): string ={
       if(i%2==0) "i is even"
       else "i is odd"
       }
       
       
Collections :
Array
Array Buffers
Maps
Tuples
Lists


Array :
val x= new Array[Int] (12)

Array Buffer:
val x= new ArrayBuffer[Int] ()

Mpas : Key valu Pairs:
val x =Map("x"-> 123, 'y'-> "42')
Both Immutable & Mutable maps are present.
.get()
.getOrElse()

To add  a key: m+=( 1-> "jenny")

 
