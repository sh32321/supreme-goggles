# Lab 1

## Q1: 
> Write a Java program with a method named 'totalSum' that takes in an argument of two integers and return its sum. Call this method from main( ) and print the results.


>Ans:

public class method {
	
	public static void totalSum(int A,int B) {
		int C=0;
		C=A+B;
		System.out.println("The total sum of "+A+" and "+B+" is " +C);

	}


	public static void main(String[] args) {
		totalSum(12, 12);

	}

}





## Q2:
> Write a Java program with a method named 'getGrades' that will display grades according to the marks entered into the method call as below:
```
Marks        Grade
91-100         A+
81-90          A-
71-80          B+
61-70          B-
51-60          C+
41-50          D-
<=40          Fail
```
>Ans:
public class method {
	
	public static void getGrades(int A) {
		char level;
		
		if(A==100 || A>=91) {
		System.out.println("A+");

			
		}
		else if(A==90||A>=81) {
		System.out.println("A-");

		}
		else if(A==80||A>=71) {
		System.out.println("B+");
		}
		else if(A==70||A>=61) {
		System.out.println("B-");
		}
		else if(A==60||A>=51) {
		System.out.println("C+");

		}
		else if(A==50||A>=41) {
		System.out.println("D-");
		}
		else {
		System.out.println("Fail");

		}
			

	}


	public static void main(String[] args) {
		getGrades(95);


	}

}

## Q3:
> Write a program to print the factorial of a number by defining a method named 'factorial'. Factorial of any number n is represented by n! and is equal to 1*2*3*....
``` 
4! = 1*2*3*4 = 24
3! = 3*2*1 = 6
2! = 2*1 = 2
Also,
1! = 1
0! = 0
```
>Ans:
public class method {
   
    public static long factorial(long number) {
        if (number <= 1)
            return 1;
        else
            return number * factorial(number - 1);
    }
    
    public static void main(String args[]) {
    for (int counter = 0; counter <= 5; counter++){
        System.out.printf("%d! = %d\n", counter,
        factorial(counter));
    }
    }
}




## Q4
> Write a Java method to create the area of a pentagon.

>Ans:
public class method {
public static double pentagon_area(int n, double s) {
        return  (n * s * s) / (4 * Math.tan(Math.PI/n));
    }

public static void main(String args[]) {
	System.out.println(pentagon_area(20,10));
}
}








