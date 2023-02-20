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
