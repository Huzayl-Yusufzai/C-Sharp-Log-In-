using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace WebsiteProgram
{
    class Program
    {
        static int tableWidth = 175;

        static void Main(string[] args)
        {
            Console.Clear();
            PrintLine();
            PrintRow("Morbius", "Popeye", "Sonic 2", "The Batman");
            PrintLine();
            PrintRow("12:45, 3:25, 6:30, 9:15", "3:00 p.m, 5:00 p.m, 7:00 p.m, 9:00 p.m", "1:00 p.m, 3:45 p.m, 6:30 p.m, 9:20 p.m", "4:30 p.m, 6:00 p.m, 8:30 p.m, 9:40 p.m");
            PrintRow("$7.99 Child, $10.99 Adult, $49.99 60+", "$7.99 Child, $10.99 Adult, $49.99 60+", "$7.99 Child, $10.99 Adult, $49.99 60+", "$7.99 Child, $10.99 Adult, $49.99 60+");
            PrintLine();
            PrintRow("Enter 1 to get seats", "Enter 2 to get seats", "Enter 3 to get seats", "Enter 4 to get seats");
            int seat = Convert.ToInt32(Console.ReadLine());
            if (seat == 1)
            {
                Console.WriteLine("Morbius seats");
            }
            else if (seat == 2)
            {
                Console.WriteLine("Popeye seats");
            }
            else if (seat == 3)
            {
                Console.WriteLine("Sonic 2 seats");
            }
            else if (seat == 4)
            {
                Console.WriteLine("The Batman seats");
            }
            else
            {
                Console.WriteLine("Invalid input");
            }


                
             Console.ReadLine();
        }

        static void PrintLine()
        {
            Console.WriteLine(new string('-', tableWidth));
        }

        static void PrintRow(params string[] columns)
        {
            int width = (tableWidth - columns.Length) / columns.Length;
            string row = "|";

            foreach (string column in columns)
            {
                row += AlignCentre(column, width) + "|";
            }

            Console.WriteLine(row);
        }

        static string AlignCentre(string text, int width)
        {
            text = text.Length > width ? text.Substring(0, width - 3) + "..." : text;

            if (string.IsNullOrEmpty(text))
            {
                return new string(' ', width);
            }
            else
            {
                return text.PadRight(width - (width - text.Length) / 2).PadLeft(width);
            }
        }           
    }
}
