using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Fishland
{
    class Fishland
    {
        static void Main(string[] args)
        {
            decimal skumriaPrice = decimal.Parse(Console.ReadLine());
            decimal cacaPrice = decimal.Parse(Console.ReadLine());
            double palamud = double.Parse(Console.ReadLine());
            double safrid = double.Parse(Console.ReadLine());
            int midi = int.Parse(Console.ReadLine());

            decimal palamudPrice = skumriaPrice * 1.60m;
            decimal safridPrice = cacaPrice * 1.80m;
            palamudPrice *= (decimal)palamud;
            safridPrice *= (decimal)safrid;
            decimal midiPrice = midi * 7.50m;

            decimal totalSum = palamudPrice + safridPrice + midiPrice;

            Console.WriteLine($"{totalSum:f2}");
        }
    }
}
