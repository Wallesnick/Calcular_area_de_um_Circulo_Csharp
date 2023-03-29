# my_lab-in-C-

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Globalization;

namespace AreaDeUmCirculo
{
    internal class Program
    {
        static void Main(string[] args)
        {
            double raio, area, pi;
            pi = 3.14159;

            Console.WriteLine("Digite o valor do raio: ");
            raio = double.Parse(Console.ReadLine(),CultureInfo.InvariantCulture);

            area = Math.Pow(raio, 2) * pi;
            Console.WriteLine("Area corresponde a : {0}", area.ToString("F4",CultureInfo.InvariantCulture));
        }
    }
}
