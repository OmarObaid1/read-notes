# error handling and debugging
Debugging is a process for testing, finding the errors and reducing them from happening in future. Debugging JavaScript either requires having support for JavaScript debugger keyword, breakpoint support with web browser tools, or third-party tools. ... Let us look at few popular debugging and error handling tools.


![](https://res.cloudinary.com/practicaldev/image/fetch/s--ewIIfR3J--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/f3meoc4rbh3xft7g8yw9.png)


# What is error handling and debugging?
Errors, bugs, and therefore debugging are a part of life for a programmer. ... Dealing with errors actually involves two very different processes: error handling and debugging. Error handling is a combination of coding and methodology that allows your program to anticipate user and other errors

# What is error handling in JavaScript?
## Error handling in JavaScript

JavaScript is a loosely-typed language. It does not give compile-time errors. ... try catch block does not handle syntax errors. JavaScript provides error-handling mechanism to catch runtime errors using try-catch-finally block, similar to other languages like Java or C#


![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRDoUzlOTAaLx3ASVxk8Mkwgv3IIOOuakeoMg&usqp=CAU)



# How do you handle errors in JavaScript?
## How to handle exceptions in JavaScript
+ A try-catch-finally statement is a code or program that handles exceptions.
+ The try clause runs the code that generates exceptions.
+ The catch clause catches exceptions that are thrown.
+ A finally clause always gets executed.
+ The throw statement generates exceptions.

# Which statement is used to handle the error?
The try statement allows you to define a block of code to be tested for errors while it is being executed. The catch statement allows you to define a block of code to be executed, if an error occurs in the try block


# Effective Error Handling and Logs
Handling Log Levels
When developing JavaScript applications it is important to have different levels of logging enabled. For example, when the application runs in testing or staging environments, it is possible to enable detailed logging including application flow, important variables & etc. while in production environments only to log errors. To achieve these, either a third-party JavaScript library or a custom implementation is required to manage log-levels.

## Log Transport
Since JavaScripts runs on client's browser, an error occurred remotely needs to be transferred to a new environment so that the development or ops team can investigate by accessing the logs.


![](https://lh6.googleusercontent.com/6IuYE7hqFkCb45_Vidh6Dcq8ls3ZM7tDgNxQzEldsLMaM1TJvT8I4gnFImdWZj9ylyLS68GXWE-F3lktiKI-FbvOIdMXiS5nzF9lAfAChr-JHZHMMEbyUnIIWbr4KrVcSYzmwGuo)

## Log Formats
It is also important to have a format which is possible to be extended in future to support any new log data formats as well as to keep uniformity across different logging messages.

## Exception Handling
This is one of the key areas, where it is required to effectively handle the errors and show users with sufficient information about the situation and pass that information to the developer. This can also be handled based on Log Levels.


lo learn more about it please join the link:

[error handling and debugging](https://dzone.com/articles/effective-debugging-and-error-handling-for-javascr)







