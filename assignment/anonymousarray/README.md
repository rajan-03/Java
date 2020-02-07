Anonymous array: An array in Java without any name is anonymous array. It is an array just for creating and using instantly.It can be further                         clarified by following points:
1) An array without name is known as anonymous array in java. 
2) As the array do not have any name so it can be used only once. 
3) Anonymous array is passed as an argument of method. 
4) Anonymous array is created and initialized in the same line.
    
            Syntax:
                    // anonymous int array 
                    new int[] { 1, 2, 3, 4};  

                      
                    new char[] {'x', 'y', 'z'); 

                   
                   new String[] {"Geeks", "for", "Geeks"}; 

                 
                     new int[][] { {10, 20}, {30, 40, 50} };
                    
      Code
             class AnonymousArray
              {
               static void print(int a[])
              {
               for(int i=0;i<a.length;++i)
               System.out.print(a[i]+" ");
              }
 
               static void print(int a[][])
              {
               for(int i=0;i<a.length;++i)
              {
               for(int j=0;j<a[i].length;++j)
               System.out.print(a[i][j]+" ");
 
               System.out.println("");
              }
              }
  
               public static void main(String...s)
             {
  
               print(new int[]{10,20,30,40});
 
              System.out.println("n");
  
 
              print(new int[][]{{10,20},{30,40},{50,60}});  
             }
             }

 
