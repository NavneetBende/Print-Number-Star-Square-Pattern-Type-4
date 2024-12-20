PRINT PATTERN  1*2*3*4  9*10*11*12
For any input number N Print the following code – For below code N=4

1*2*3*4
9*10*11*12
13*14*15*16
5*6*7*8
PREREQUISITE:
Basic knowledge in Java programming, usage of loops.

ALGORITHM:
Take input from user i.e number of lines required (N value).
Take two loops one for each line (say ‘i’) and other for each digit in a particular line (say ‘j’). i starts from 1 and j starts from 1.
Take a result variable (say ‘m’) and initialize it with 1.
Here ‘i’ loop is used to access each line from 1 to n-1 and ‘j’ loop is used to print values in each line. First j loop executes when i not equal to 1 and other j loop runs in remaining cases.
Print ‘m’ value along with * and post increment  until the j loop reaches a value less than n.
Print the final value ‘m’ of each line.
Repeat the ‘i’ loop until it reaches n-1.
CODE IN JAVA:
[code language=”java”]
import java.lang.*;
import java.io.*;
class Pattern
{
public static void main(String[] args)throws IOException
{
BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
int n,i,j,m=1;
System.out.print("Enter N value:");
n=Integer.parseInt(br.readLine());
for(i=1; i<=n-1; i++)
{
if(i!=2)
{
for(j=1; j<n; j++){
System.out.print((m++)+"*");
}
System.out.print(m++);
System.out.println();
}
else {
m = m+n;
for(j=1; j<n; j++){
System.out.print((m++)+"*");
}
System.out.print(m++);
System.out.println();
}
}
for(i=n+1 ;i<(n+n);i++){
System.out.print(i+"*");
}
System.out.print(i);
System.out.println();
}
}
[/code]

TAKING INPUT:


DISPLAYING OUTPUT:
