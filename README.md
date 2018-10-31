# Bubble-Sort
Integer sort

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace mid_prep
{
    class Program
    {
       class Sort
        {
            public static void ascSort (int [] array)
            {
                int temp;
                for (int i = 0; i < array.Length; i++)
                {
                    for (int j = 0; j < array.Length; j++)
                    {
                        if (array[j]>array[i])
                        {
                            temp = array[j];
                            array[j] = array[i];
                            array[i] = temp;
                        }
                    }
                }
                foreach (var element in array)
                {
                    Console.WriteLine(element);
                }
            }
        }
        
        static void Main(string[] args)
        {
            int[] num = { 10, -5, 3, 21, -1, 84, 112, 5, 238, 44 };
            Sort.ascSort(num);
        }
    }
}
