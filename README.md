TestCar
=======
import java.io.*;

class Vehicle
{
    public void move()throws Exception
	{
        System.out.println("Vehicle can move");
    }
}

class Car extends Vehicle
{
    public void move()
	{
        System.out.println("A car is a four wheeler");
    }
}

public class TestCar
{
    public static void main(String args[])
	{
        Vehicle a = new Vehicle(); // Vehicle reference and Vehicle object
        Vehicle b = new Car(); // Vehicle reference but Car object

		try
		{
            a.move();// runs the method in Vehicle class
            b.move();//Runs the method in Car class
		}
		
		catch(Exception e)
		{
		    e.printStackTrace();
		}
    }
}
