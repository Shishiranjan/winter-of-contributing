Before We dive deep into the typecasting it is mandatory to understand the concept of type conversion because typecasting actually solves the problem of typeconversion.

# Type Conversion:
When one type of data is assigned to another type of variable, then automatically type conversion will take place. But for type conversion to happen the following conditions should met:

# 1: The two datatypes must be compatible.
Compatible in the sense that both the datatype should be treated as the same although it's value is different. For ex: 30 and 30.0. Here both 30 and 30.0 are the same thing of course. It means that both int and float datatypes are compatible.

```Javascript
int num1 = 30;
float num2 = 30.0;
```

So, if i specify to take the float value in the code which in this case is 30.0, but if we take int value from the user then the compiler automatically convert that int datatype to float datatype and error is not thrown in the console.

# 2: The destination datatype should be greater than the source datatype.
If the datatype which you are asking is greater than in terms of size than that of the datatype which you're giving to the code, then in that case onle type conversion works.

# Note:
Type conversion automatically happens in the case of datatypes like long, double, char, short, float etc.

But What happens if the datatype which you are asking is less in terms of size than that of the datatype which you are giving. Is there a solution for this ? And the answer is yeah.

And here Type casting comes into picture.

# Type casting
Type casting actually compress the bigger number associated with the dataype which is greater in terms of it's size as compared to the smaller number associated to the datatype which is less in terms of it's size. Here the size simply means that how much byte of memory any datatype takes.

In simple words, Type casting is simply the compressing of bigger number to smaller number and also smaller number to bigger number. Only difference is that the compression of smaller number to bigger number is done automatically by the compiler whereas the compression of bigger number to smaller number is done manually. So, With this above statement we know that Type casting is of two types:

# 1: Widening Casting

Widening casting is done automatically when we pass a smaller number having the datatype that is less in size and wants to print the the same number but with another datatype that is bigger in size. Take a look at this sample of code to understand this;

```Javascript
public class main {
public static void main(String[] args){
int num1 = 47;
double num2 = num1; // Here the type casting is done from int to double i.e. from smaller number to bigger number.

    System.out.println(num1);      // 47 is printed here.
    System.out.println(num2);   // 47.0 is printed here.
  }
}

```
# 2 Narrowing Casting

Narrowing casting is done automatically when we pass a bigger number having the datatype that is greater in size and wants to print the the same number but with another datatype that is less in size. And this type casting is done manually by the user.

Again let's make it clear from this sample of code:

```Javascript
public class Main {
public static void main(String[] args) {
    double num1 = 39.56d;
    int num2 = (int) num1; // Here casting is done manually.

    System.out.println(num1);   // Here 39.56 was printed.
    System.out.println(num2);      // Here 39 was printed.
  }
}
```
