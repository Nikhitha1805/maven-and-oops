import java.io.*;

abstract class Operation
{

    
    //abstract void getdata();

    abstract void oper();

}

class Add extends Operation
{

    private int a,b;
   
 public void oper()
  
  {
        System.out.println("Add of two num is"+(a+b));

    }

}

class Sub extends Operation
{
  
  private int a,b;

    public void oper()
 
   {
        System.out.println("Sub of two num is"+(a-b));

    }

}

class Mul extends Operation

{

    private int a,b;

    public void oper()

    {
        
System.out.println("Mul of two num is"+(a*b));
 
   }

}

class Div extends Operation
{

    private int a,b;
   
 public void oper()
    
{

        System.out.println("Div of two num is"+(a/b));

    }

 
class ArithmeticTest

{

    public static void main(String args[])
   
 {

        Scanner sc=new Scanner(System.in);
   
     Shape s;

        System.out.println("Enter choice 1-Addition 2-Subtraction 3-Multiplication 4-Division");
 
       int ch=sc.nextInt();
  
      System.out.println("Enter number");

        int a=sc.nextInt();

        System.out.println("Enter another number");
   
     int b=sc.nextInt();
  
      if(ch==1)
   
         s=new Add();
   
     else if(ch==2)
    
        s=new Sub();

        else if(ch==3)
    
        s=new Mul();
   
     else if(ch==4)
   
         s=new Div();

        s.oper();

        
        
    }

}