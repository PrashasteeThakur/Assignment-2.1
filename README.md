# Assignment-2.1
1.
public class acad{
public static void main(String[] args){
int a=5;  //1st number
int b=4;  //2nd number
int c;
c=a+b;    //sum of two numbers
System.out.println(c); //displays sum
}
}


2.
import java.util.*;
public class acad{
public static void main(String[] args){
Scanner sc=new Scanner(System.in);
int a=sc.nextInt();   //1st number from user
int b=sc.nextInt();   //2nd number from user
int c;
c=a+b;                //sum of two numbers
System.out.println(c); //displays sum
sc.close();
}
}


3.
import java.util.*;
public class acad{
public statc void main(String[] args){
sum();
}
public static void sum()
{
Scanner sc=new Scanner(System.in);
int a=sc.nextInt();   //1st number from user
int b=sc.nextInt();   //2nd number from user
int c;
c=a+b;                //sum of two numbers
System.out.println("First number is:"+a);  //displays 1st number
System.out.println("Second number is:"+b); //displays 2nd number
System.out.println("Sum is:"+c);   //displays sum
sc.close();
}
}

4.
import java.util.*;
public class acad{
public static void main(String[] args){
Scanner sc=new Scanner(System.in);
int a=sc.nextInt();   //1st number from user
int b=sc.nextInt();   //2nd number from user
System.out.println("Even numbers are:");
for(int i=a;i<=b;i++)
{
if(i%2==0)       //check if even
{
System.out.println(i);   //displays even numbers
}
}
System.out.println("Odd numbers are:");
for(int i=a;i<=b;i++)
{
if(i%2!=0)      //check if odd
{
System.out.println(i);   //displays odd numbers
}
}
}
}

5.
import java.util.*;
public class acad{
public static void main(String[] args){
Scanner sc=new Scanner(System.in);
int a=sc.nextInt();   //number from user
for(int i=1;i<=10;i++)
{
System.out.println(a+"x"+i+"="+(a*i));  //displays 1st 10 multiples of a
}
}
}

6.
import java.util.*;
public class acad{
public static void main(String[] args){
Scanner sc=new Scanner(System.in);
int a=sc.nextInt();   //1st number from user
int b=sc.nextInt();   //2nd number from user
int c=sc.nextInt();   //3rd number from user
sum(a,b);
sum(a,b,c);
}
//method overloading
public static void sum(int a,int b)
{
System.out.println("Sum of first 2 numbers is:"+(a+b));
}
public static void sum(int a,int b,int c)
{
System.out.println("Sum of all 3 numbers is:"+(a+b+c));
}
}


7.
The method should be overloaded with the same return type in order to
avoid ambiguity.
For example,
class A{
static int add(int a,int b){return a+b;}
static double add(int a,int b){return a+b;}
}
class B{
public static void main(String[] args){
System.out.println(Adder.add(11,11));//ambiguity
}}
In this when code is compiled it will show error as:
Overloading3.java:3: error: method add(int,int) is already defined in class A
static double add(int a,int b){return a+b;}

To overcome this problem method should be overloaded with the same return type.


8.
import java.util.*;
public class acad{
public static void main(String[] args){
Scanner sc=new Scanner(System.in);
int n=sc.nextInt();   //size of array
int[] a=new int[n];
for(int i=0;i<n;i++)
{
a[i]=sc.nextInt();
}
Arrays.sort(a);   //sorting array
for(int i=a.length-1;;i>=0;i--){
System.out.println(a[i]+" ");  //displaying sorted reversed order array elements
}
}
}
