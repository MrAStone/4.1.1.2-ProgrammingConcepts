<pre lang=c#>
using System;
using System.Collections.Generic;
using System.Data;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._1._1._2_ProgrammingConcepts
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //Use, understand and know how the following
            //statement types can be combined in programs:
            //• variable declaration
            int intIdentifier;
            string stringIdentifier = "This is a string";

            //• constant declaration
            const int neverChanges = 42;
            //• assignment
            intIdentifier = 12;
            stringIdentifier = Console.ReadLine();
            //• iteration
            for (int i = 0; i < 10; i++)
            {
                Console.WriteLine(i);
            }
            foreach (char c in stringIdentifier)
            {
                Console.WriteLine(c);
            }
            int x = 1;
            do
            {
                x++;
            } while (x < 10);

            while (x > 1)
            {
                x--;
            }
            x = 0;
            do
            {
                x += 3;
            } while (x != 30);
            //• selection
            if (x != 1)
            {
                Console.WriteLine("Not 1");
            }
            if (x != 2)
            {
                Console.WriteLine("Not 2");
            }
            else
            {
                Console.WriteLine(2);
            }
            if (x != 3)
            {
                Console.WriteLine("Not 3");
            }
            else if (x != 4)
            {
                Console.WriteLine("Not 4");
            }
            else
            {
                Console.WriteLine("3 or 4");
            }
            //• subroutine(procedure / function).
            // Calling function
            Console.WriteLine(anIntFunction());
            // Calling procedure
            aProcedure();
            //Calling function with parameters
            Console.WriteLine(aStringFunctionWithParameters("hello"));
            //calling a procedure with parameters
            aProcedureWithParameters("hello");

            //Use nested selection and nested iteration
            //structures.
            Console.WriteLine("Nested For Loops");
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    Console.WriteLine($"{i} {j}");
                }
            }
            Console.WriteLine("For and While nested");
            for (int i = 0; i < 10; i++)
            {
                Console.Write("Enter a word: ");
                string input = Console.ReadLine();
                while (input == "")
                {
                    Console.Write("Enter a word: ");
                    input = Console.ReadLine();
                }
            }

        }
        static int anIntFunction() // define data type of return
        {
            return 5;
        }
        static void aProcedure()// procedures return void
        {
            Console.WriteLine("Procedure has been called");
        }
        static string aStringFunctionWithParameters(string param)
        {
            return param + param;
        }
        static void aProcedureWithParameters(string input)
        {
            Console.WriteLine(input + input);

        }
    }
}
            </pre>
