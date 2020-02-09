  An interface which is declared inside another interface or class is called nested interface.   They are also known as inner interface. Since nested interface cannot be accessed directly,    the main purpose of using them is to resolve the namespace by grouping related interfaces      related interface and class) together.  This way, we can only call the nested interface by     using outer class or outer interface name followed by dot( . ), followed by the interface      name

   Example: Entry interface inside Map interface is nested. Thus we access it by calling Map.Entry.
          
  The following are the rules governing a nested interface.

   A nested interface declared within an interface must be public.
      A nested interface declared within a class can have any access modifier.
      A nested interface is by default static 
                      
                          code
                          
      public class Demo1 {
      public static void main(String[] args){
      C ob = new C();
      ob.method();
    }
    }
 
      class A{
    
      protected interface B{
      void method();
    }
    }
 

     class C implements A.B{
     public void method() {
     System.out.println("Demo: interface nested inside a class");
    }
    }
	
      Output : Demo: interface nested inside a class
