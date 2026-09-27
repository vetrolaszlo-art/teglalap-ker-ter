using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace alapok1
{
    internal class Program
    {
        //függvény, eljárás
        public static void feladat1()
        {
            Console.Write("Első szám:");
            int a = Convert.ToInt32(Console.ReadLine());

            Console.Write("Második szám:");
            int b = Convert.ToInt32(Console.ReadLine());

            int osszeg = a + b;
            Console.WriteLine($"A két szám összege: {osszeg}");
        }

        static void feladat2()
        {
            Console.Write("Hosszúság:");
            double hossz = Convert.ToDouble(Console.ReadLine());
            Console.Write("Szélesség:");
            double szel = Convert.ToDouble(Console.ReadLine());

            double kerulet = 2 * (hossz + szel);
            Console.WriteLine($"A téglalap kerülete: {kerulet}");

            double terület = hossz * szel;
            Console.WriteLine($"A téglalap területe: {terület}");
        }

        static void feladat3(int eddig)
        {
            List<int> list = new List<int>();
            for (int i = 0; i < eddig; i++)

            {
                Console.Write($" {i + 1}. szám: ");
                list.Add(Convert.ToInt32(Console.ReadLine()));
            }
            Console.Write("A megadott számok: ");
            foreach (int i in list)
            {
                Console.Write(i.ToString() + " ");
            }
            Console.Write("\n");
            Console.WriteLine(list.Sum());
          

        }
        static void Main(string[] args)
        {
            #region 1.feladat
            Class2.feladat1();
            #endregion

            #region 2.feladat
            feladat2();
            #endregion

            #region 3.feladat
            Console.Write("Hány számot szeretne megadni? ");
            int db = Convert.ToInt32(Console.ReadLine());
            //feladat3(db);
            #endregion

            #region 4.feladat
            Console.Write("Adja meg a számot ");
            int szam = Convert.ToInt32(Console.ReadLine());
            for ( int i = 0;i < szam;i++)
            { 
                Console.WriteLine(i + 1);

            }
            #endregion


            #region 5.feladat
            #endregion
        }
    }
}
