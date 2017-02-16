# Assignment-2.1
Ques.(g) Can you overload a method with the same return type? Explain your
answer with proper logic.

Ans.(g)
The method should be overloaded with the same return type in order to
avoid ambiguity.
For example,
class A{
static int add(int x,int y)
{
return x+y;
}
static long add(int x,int y)
{
return x+y;
}
}
class B{
public static void main(String[] args){
System.out.println(Adder.add(11,11));    //ambiguity
}}
Exception in thread "main" java.lang.Error: Unresolved compilation problem: 
	Adder cannot be resolved

	at acad.main(acad.java:15)

To overcome this problem method should be overloaded with the same return type or with different number of parameters.
