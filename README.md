# Exception-Handling

Exception handling is a crucial part of Java programming as it allows developers to anticipate and respond to errors and other exceptional events that may occur during program execution. In this article, we will discuss exception handling in Java in medium depth. 

# What is an Exception?

In Java, an exception is an event that interrupts the normal flow of program execution. Exceptions can occur due to a variety of reasons such as input errors, resource exhaustion, network failures, and so on. When an exception occurs, the program terminates abruptly unless we handle it properly.

# Exception Handling in Java

Exception handling in Java involves the following steps:

1. Detecting Exceptions: In Java, exceptions are detected automatically by the JVM or explicitly using the throw statement.

2. Handling Exceptions: Once an exception is detected, we have to handle it properly to avoid abrupt termination of the program. Java provides four types of exceptions that can be used to handle exceptional events:

 a. try-catch: This block is used to catch exceptions that occur in the try block and handle them appropriately.

 b. throw: This statement is used to throw exceptions explicitly when a certain condition occurs.

 c. throws: This clause is used to declare the exception that can be thrown by the method or class.

 d. finally: This block is used to execute any code that needs to be executed regardless of the occurrence of an exception.

3. Propagating Exceptions: Sometimes, we may want to propagate the exception to another part of the program instead of handling it in the current block. In such cases, we can use the throws clause to declare the exception and throw statement to pass it to the calling method.

# Best Practices for Exception Handling in Java

Here are some best practices for exception handling in Java that developers can follow to write robust and maintainable code:

1. Use specific exception classes to handle specific errors and avoid catching the base Exception class.

2. Keep the try block as small as possible and minimize the code inside it.

3. Always include a catch block after the try block to handle the exceptions.

4. Avoid catching exceptions that you cannot handle.

5. Use finally block to close resources and perform any cleanup operations.

6. Do not suppress exceptions and log them instead.

# Conclusion

Exception handling is a critical aspect of Java programming. By following the best practices listed above, developers can write programs that are more robust and maintainable, and handle exceptional events gracefully.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------

# throw vs throws

//Java throw example
void a()
{
  throw new ArithmeticException("Incorrect");
}
//Java throws example
void a()throws ArithmeticException
{
  //method code
}
//Java throw and throws example
void a()throws ArithmeticException
{
  throw new ArithmeticException("Incorrect");
}
