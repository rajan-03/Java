  Exception class
   If we are creating your own Exception that is known as custom exception or user-defined exception. Java custom exceptions are used to customize the exception according to user need.
  By the help of custom exception, we can have your own exception and message.
                       
 Method for creating exception class
   We should  create a new class whose name should end with Exception like ClassNameException. This is a convention to differentiate an exception class from regular ones.Then,we should    make  the class that extends one of the exceptions which are subtypes of the    java.lang.Exception class. Generally, a custom exception class always extends directly from    the Exception class.Then we should create a constructor with a String parameter which is    the detail message of the exception. In this constructor, simply we should call the super    constructor and pass the message
                     
                     code
                     
          class InvalidAgeException extends Exception{  
          InvalidAgeException(String s){  
          super(s);  
        }  
        }  
         class TestCustomException1{  
  
         static void validate(int age)throws InvalidAgeException{  
         if(age<18)  
         throw new InvalidAgeException("not valid");  
         else  
         System.out.println("welcome to vote");  
     }  
     
        public static void main(String args[]){  
        try{  
        validate(13);  
       } catch(Exception m){System.out.println("Exception occured: "+m);}  
  
         System.out.println("rest of the code...");  
    }  
    }
        Output:Exception occured: InvalidAgeException:not valid
               rest of the code...
