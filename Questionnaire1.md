Java Questionnaire - 1

Topics : Data types, OOP


NOTE : 
1. Explain the output of below programs . If there is a compilation error mention the line causing compiler error and add corrected code and then Explain the output.
2. Create another Ans1.md file and write all corrected code and answers
3. Code below has been executed and tested, however there can be some intentional errors.
 

QUESTIONS :

1.

class MainClass {
	public static void main(String[] args) {
		
		char a = 'G' + ‘A’;
		a = (char) (a + '9');
		System.out.println(a);
	}
}

#2

class MainClass {
	public static void main(String[] args) {
		
		System.out.println((char)128);
		System.out.println((int)' ');
		System.out.println((int)'	');
		System.out.println((int)'\n');
		System.out.println(int);
		System.out.println(true);
	}
}

#3


class MainClass {
	public static void main(String[] args) {
		
		int arr1[] = {1,2,3};
		int arr2[] = {1,2,'3'};
		

		for(int i=1;i<arr1.length;i++){
			arr1[i]+=arr1[i-1];
			arr2[i]+=arr2[i-1];
		}
		
		System.out.println(Arrays.toString(arr1));
		System.out.println(Arrays.toString(arr2));
		
		
		char ar1[] = {16,53,67};
		char ar2[] = {15,45,'3'};
		

		for(int i=1;i<arr1.length;i++){
			ar1[i]+=ar1[i-1];
			ar2[i]+=ar2[i-1];
		}
		
		System.out.println(Arrays.toString(ar1));
		System.out.println(Arrays.toString(ar2));
	}
}


#4 

public class MainClass {
	int t2 ;
	static int t3;
	public static void main(String[] args) {
		int t ;
		System.out.println(t);
		System.out.println(t=0);
		System.out.println(MainClass.t3);
		System.out.println(new MainClass().t2);
	}
}

#5


public class MainClass {
	
	public static void main(String[] args) {
		byte byt = (byte) 129;
		byte byt1 = (byte) 128;
		byte byt2 = (byte) 123;
		System.out.println(byt);
		System.out.println(byt1);
		System.out.println(byt2);
			
	}
}


#6



class M
{
    static
    {
        System.out.println('A');
    }
 
    {
        System.out.println('B');
    }
 
    public M()
    {
        System.out.println('C');
    }
}
 
class N extends M
{
    static
    {
        System.out.println('D');
    }
 
    {
        System.out.println('E');
    }
 
    public N()
    {
        System.out.println('F');
    }
}
 
public class MainClass
{
    public static void main(String[] args)
    {
        N n = new N();
    }
}

Additional Question 1 : What is the difference between a static block and an initialiser block.?
Additional Question 2 : What is the order of execution of : 
					1. Static Block
					2. Initialiser Block
					3. Constructor



#7 


class A {
	 int x = 9;
	A() {
		x = 0;
		System.out.println("The value of x : " + x);
	}
}
class B extends A{
	
	B() {
		x = 8;
		System.out.println("The value of x = "+x);
	}
}

public class MainClass
{
    public static void main(String[] args)
    {
        new B();
    }
}


Additional Questions : 
	1.  What is the order in which both constructors are loaded and executed by the JVM.?
	2.  What happens if parent and child class both have a variable of the same name and type?
	3. How can both of these variables be accessed ?


#8
Explain the output of both code snippets.

1. MainClass.java

class A {
static int x = 9;
static {
	x = 0;
	System.out.println("The value of x : " + x);
}
}
class B extends A{
	static int x = 19;
	static {
		
		System.out.println("The value of x = "+x);
	}
}


public class MainClass
{
   static {
	System.out.println(“Main Class”);
   }
   public static void main(String[] args)
   {
       
   }
}

2. MainClass1.java
class A {
	static int x = 9;
	static {
		x = 0;
		System.out.println("The value of x : " + x);
	}
}
class B extends A{
	static int x = 19;
	static {
		//x = 8;
		System.out.println("The value of x = "+x);
	}
}


public class MainClass1
{
   public static void main(String[] args)
   {
       System.out.println(A.x);
   }
}

3. MainClass2.java
class A {
	static int x = 9;
	static {
		x = 0;
		System.out.println("The value of x : " + x);
	}
}
class B extends A{
	static int x = 19;
	static {
		//x = 8;
		System.out.println("The value of x = "+x);
	}
}


public class MainClass2
{
   public static void main(String[] args)
   {
       System.out.println(B.x);
	
   }
}



Additional Questions : 
	1.  What is the order in which both static blocks  are loaded and executed by the JVM ?
	2.  What happens if parent and child class both have a variable of the same name and type?
    3.  How can both of these variables be accessed?














