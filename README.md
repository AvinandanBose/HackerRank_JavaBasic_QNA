# HackerRank_JavaBasic_QNA
This is a repository which discusses about the question and answers of Java Basic Certificate


<h3>Q1) Write a Comparator class with the following overloaded compare methods:</h3>
<h3><li>1.boolean compare(int a, int b):Return true if int a = int b otherwise return false.</li></h3>
<h3><li>2.boolean compare(String a, String b):Return true if String a = String b otherwise return false.</li></h3>
<h3><li>3.boolean compare(int[] a, int[] b):Return true if int[] a = int[] b otherwise return false.</li></h3>
<ul>
<h3><li>3.a)Arrays a and b are of equal length.</li></h3>
<h3><li>3.b)For  each index i( where 0 < = i < a.length ) a [ i ] = b [ i ]. </li></h3>
</ul>


<h3 align=left>

```
class Comparator{

//boolean compare(int a, int b):Return true if int a = int b otherwise return false.

boolean compare(int a, int b){

if(a == b){
    return true;
  }

return false;

}

//boolean compare(String a, String b):Return true if String a = String b otherwise return false.

boolean compare(String a, String b){

if(a == b){
    return true;
  }

return false;

}

+++++++++++++++++++++++++++++++
//boolean compare(int[] a, int[] b):Return true if int[] a = int[] b otherwise return false.
//Arrays a and b are of equal length.
//For  each index i( where 0<=i<a.length) a[i] = b[i].
++++++++++++++++++++++++++++

 boolean compare(int[] a, int[] b){
 
 //Now check arrays are of equal length 
  if (a.length != b.length) {
          return false;
    }
    
    //Return true if int[] a = int[] b otherwise return false
    //For  each index i( where 0<=i<a.length) a[i] = b[i].
    
    for (int i = 0; i < a.length; i++) {
            if (a[i] == b[i]) {
                return true;
             }
       }
       return false;
       
     }
 
 
 }


```
</h3>

<h3>Q2) Given a bare class, Arithmetic write a method sum, that accepts an array as an argument. Overload it to the process an array of Integer or String types as follows: For an Integer array, return the sum of the elements and For a String array, concatenate string in order.</h3>


<h3 align=left>

```

public class Arithmetic {

    // Method to sum the elements of an Integer array
    public static int sum(Integer[] arr) {
        int sum = 0;
        for (int i = 0; i < arr.length; i++) {
            sum += arr[i]; //Sum of Elements
        }
        return sum;
    }

    // Method to concatenate the elements of a String array
    public static String sum(String[] arr) {
        StringBuilder sb = new StringBuilder();
        for (int i = 0; i < arr.length; i++) {
            sb.append(arr[i]); //concatenate the elements of a String
        }
        return sb.toString();
    }
}


```
</h3>

<h3>Q3) Below is the Question, what will be the result ?</h3>

<h3 align=left>

```
class A{
    public int add(int a, int b){
        return a+b;
    }
    public static void main(String[] args){
        A a = new A();
       short s= 9;
       System.out.println(a.add(s,6))
    }
}


```
</h3>

<h3> Ans: 15 , Reason: The casting occurs here is <ins>Widening Casting </ins>,In Widening Casting(byte -> short -> char -> int -> long -> float -> double) , hence int can hold a char value , short value and a byte value . </h3>

