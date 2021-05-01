using System;

namespace Csharp
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Type the name of your fav shape from the following: square, circle, rectangle, triangle");
            string shape = Console.ReadLine();

            if (shape == "square")
            {
                Console.WriteLine("You picked 'square'. Type the side lenght of the shape (use numbers only): ");
                string side = Console.ReadLine();
                int sqside = 0;
                try
                {
                    sqside = Int32.Parse(side);
                    int sqcircumf = 4 * sqside;
                    int sqarea = sqside * sqside;

                    Console.WriteLine($"Square's circumference is '{sqcircumf}' and area '{sqarea}'");
                }
                catch
                {
                    Console.WriteLine($"Something wrong with the input - '{side}'. Did you use numbers here?");
                }


            }
            else if (shape == "circle")
            {
                {
                    {
                        double mittTal; 
                        Console.Write("Cirkelns radie: "); 
                        mittTal = double.Parse(Console.ReadLine()); 

                        Console.WriteLine("Area= " + mittTal * 2 * Math.PI); 

                        Console.WriteLine("cirkum= " + mittTal * mittTal * Math.PI);


                        }

                    
                        }

            }
            else if (shape == "rectangle")
                        {
                
                {
                    {
                        Console.WriteLine("Enter length of rectangle:");
                    double rectangleLength = Convert.ToDouble(Console.ReadLine());

                    Console.WriteLine("Enter width of rectangle:");
                    double rectangleWidth = Convert.ToDouble(Console.ReadLine());

                    double areaOfRectangle = rectangleLength * rectangleWidth;
                    Console.WriteLine("Area of rectangle is: " + areaOfRectangle);

                    double circumferenceOfRectangle = 2 * (rectangleLength) + 2 * (rectangleWidth);
                    Console.WriteLine("Circumference of rectangle is: " + circumferenceOfRectangle);

                    }


                }
            }
            
                 else if (shape == "triangle")
                {
                    Console.WriteLine("Enter the side1 of triangle:");
                    double triangleSide1 = Convert.ToDouble(Console.ReadLine());
                    Console.WriteLine("Enter the side2 of triangle:");
                    double triangleSide2 = Convert.ToDouble(Console.ReadLine());
                    Console.WriteLine("Enter the side3 of triangle:");
                    double triangleSide3 = Convert.ToDouble(Console.ReadLine());
                    double circumferenceOfTriangle = triangleSide1 + triangleSide2 + triangleSide3;
                    Console.WriteLine("Circumference of triangle is: " + circumferenceOfTriangle);

                }
            }
        }

}

