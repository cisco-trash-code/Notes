# Java Notes

## General


- In Java, every value is either a reference to an object, or it belongs to one of the eight Floating-point numbers have limited precision. Not every value can be represented precisely,
and roundoff errors can occur.
primitive types.

- A final variable is a constant. Once its value has been set, it cannot be changed. Many programmers use all-uppercase names for constants. That way, it is easy to distinguish between variables and constants.
  
- Frequently, constant values are needed in several methods. Then you should declare them together with the instance variables of a class and tag them as static and final.
  ```
    // Declared in a maethod 
    // final typeName variableName = expression;
    final double NICKEL_VALUE = 0.05;

    // Declared in a class
    // accessSpecifier ststic final typeName variableName = expression;
    public static final double LITERS_PER_GALLON = 3.785;
    ```

- If you want to compute with really large numbers, you can use big number objects. Big number objects are objects of the **BigInteger** and **BigDecimal** classes in the java.math package. Unlike
the number types such as int or double, big number objects have essentially no limits on their
size and precision. However, computations with big number objects are much slower than
those that involve number types. Perhaps more importantly, you can’t use the familiar arithmetic operators such as (+ - *) with them. Instead, you have to use methods called add, subtract, and multiply.

- A method that accesses an object and returns some information about it, without changing the
object, is called an **accessor method**. In contrast, a method whose purpose is to modify the internal data of an object is called a **mutator method**.

- The public interface of a class specifies what you can do with its objects. The hidden implementation describes how these actions are carried out.

- Calling one constructor from another
  ```
    public class BankAccount{
        public BankAccount(double initialBalance){
            balance = initialBalance;
        }
        public BankAccount(){
            this(0);
        }
        . . .
    }
    ```
    The command this(0); means “Call another constructor of this class and supply the value 0”.


## OOP

- Constructors set the initial data for objects.
  
- When a method exits, its local variables are removed.
  
- Instance variables are initialized to a default value, but you must initialize local variables.
  
- Encapsulation is the process of hiding implementation details and providing methods for data access. Encapsulation allows a programmer to use a class without having to know its
implementation.

