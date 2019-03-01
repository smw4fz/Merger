using System;
using System.Collections;
using System.IO; 

namespace Merge
{
    class Program
    {
        static void Main(string[] args)
        {

            do
            {
                Console.WriteLine("~ DOCUMENT MERGER ~");
                Console.WriteLine("What is the name of the first file?");
                string doc_1 = Console.ReadLine();
                string checkFile = @"c:\doc_1.txt";
                Console.WriteLine(File.Exists(checkFile) ? "File exists." : "File does not exist.");

                Console.WriteLine("What is the name of the second file?");
                string doc_2 = Console.ReadLine();
                string checkFile2 = @"c:\doc_2.txt";
                Console.WriteLine(File.Exists(checkFile2) ? "File exists." : "File does not exist.");
                Console.WriteLine("Try again.");
                doc_2 = Console.ReadLine();

                StreamWriter sw = new StreamWriter("C:\\doc_1.txt\\doc_2.txt");

                int length = doc_1.Length + doc_2.Length;

                try
                {
                    sw.Close();
                }
                catch (Exception e)
                {
                    Console.WriteLine("Exception: " + e.Message);
                }
                finally
                {
                    Console.WriteLine("{0} {1} was successfully saved. The document contains {2} characters.", doc_1, doc_2, length);

                }

                Console.WriteLine("Would you like to merge another file? (yes/no)");

            } while (Console.ReadLine().ToLower().Equals("yes"));

           
        } // end main
    }
}
