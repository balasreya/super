# super
import java.util.*;
class figure
{
    int l,w;
    figure(int x,int y)
    {
        l=x;
        w=y;
    }  
    void area()
    {
        System.out.println("area of figure");
    }
}
        
    class Triangle extends figure
    {
        Triangle(int d,int h)
        {
            super(d,h);
        }
        void area()
        {
            System.out.println("area of triangle"+(l*w)); 
        }
    }
    class Rectangle extends figure
    {
        Rectangle(int b,int w)
        {
            super(b,w);
        }
        void area()
        {
             System.out.println("area of rectangle"+(l*w)/2);
        }
    }
class Main
{
    public static void main(String[] args)
    {
      Triangle ob1=new Triangle(20,40);
      ob1.area();
      Rectangle ob2=new Rectangle(20,40);
      ob2.area();
      
    }
}
