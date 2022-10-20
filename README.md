# Aasignment.java
//define a class Geometry

public class Geometry

{

// method to calculate the volume of a sphere.

public static double sphereVolume(double r)

{

//return the calculated value

return 4.0 / 3.0 * Math.PI * Math.pow(r, 3);

}

//method to calculate the surface area of a sphere.

public static double sphereSurface(double r)

{

//return the calculated value

return 4.0 * Math.PI * r * r;

}

// method to calculate the volume of a cylinder.

public static double cylinderVolume(double r, double h)

{

//return the calculated value

return Math.PI * r * r * h;

}

// method to calculate the surface area of a cylinder.

public static double cylinderSurface(double r, double h)

{

//return the calculated value

return 2 * Math.PI * r * (r + h);

}

//method to calculate the volume of a cone.

public static double coneVolume(double r, double h)

{

//return the calculated value

return 1.0 / 3.0 * Math.PI * r * r * h;

}

// method to calculate the surface area of a cone.

public static double coneSurface(double r, double h)

{

//return the calculated value

return Math.PI * r * r + Math.PI * r * Math.sqrt(r * r + h * h);

}

}

Filename: “GeometryDemo.java”

//import the required packages

import java.util.Scanner;

//define the class GeometryDemo

public class GeometryDemo

{

//define the main method

public static void main(String[] args)

{

//declare an object of the Scanner class

Scanner in = new Scanner(System.in);

//prompt the user to enter the radius

System.out.println("Enter radius: ");

//scan for the value

double radius = in.nextDouble();

//prompt the user to enter the height

System.out.println("Enter height: ");

double height = in.nextDouble();

//print the volume of Sphere

System.out.println("Sphere volume: " + Geometry.sphereVolume(radius));

//print the surface of Sphere

System.out.println("Sphere surface: " + Geometry.sphereSurface(radius));

//print the volume of Cylinder

System.out.println("Cylinder volume: "

+ Geometry.cylinderVolume(radius, height));

//print the surface of Cylinder

System.out.println("Cylinder surface: "

+ Geometry.cylinderSurface(radius, height));

//print the volume of Cone

System.out.println("Cone volume: " + Geometry.coneVolume(radius, height));

//print the surface of Cone

System.out.println("Cone surface: "

+ Geometry.coneSurface(radius, height));

}

}
