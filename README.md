       using System;
       using System.Collections.Generic;
       using System.Linq;
       using System.Text;
       using System.Threading.Tasks;

       namespace  Program35
       {
        internal class Program
       {
        static void Main(string[] args)
        {

            Console.Write("Введите значение для int: ");
            string s1 = Console.ReadLine();

            Console.Write("Введите значение для double: ");
            string s2 = Console.ReadLine();

            Console.Write("Введите значение для bool: ");
            string s3 = Console.ReadLine();

            // Проверяем и выводим результаты TryParse
            bool res1 = int.TryParse(s1, out int r1);
            Console.WriteLine($"int.TryParse: {res1} (результат: {r1})");

            bool res2 = double.TryParse(s2, out double r2);
            Console.WriteLine($"double.TryParse: {res2} (результат: {r2})");

            bool res3 = bool.TryParse(s3, out bool r3);
            Console.WriteLine($"bool.TryParse: {res3} (результат: {r3})");
        }
    }
    }
