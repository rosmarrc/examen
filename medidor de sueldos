using System;

namespace medidor_de_sueldos
{
    class Program
    {
        static void Main(string[] args)
        {
            
            string[] empleados = new string[5];
            int[] sueldo = new int[5];
            Cargar(ref empleados, ref sueldo);
            SalarioMayor(ref sueldo, ref empleados);

            Console.ReadKey();


        }
        static void Cargar(ref string[] empleados, ref int[] sueldo)
        {
            for (int contador = 0; contador < 5; contador++)
            {
                Console.Clear();
                Console.WriteLine("introduce el nombre:");
                empleados[contador] = Console.ReadLine();
                Console.WriteLine("introduce el sueldo:");
                sueldo[contador] = Convert.ToInt32(Console.ReadLine());
            }
        }

        static void SalarioMayor(ref int[] sueldo, ref string[] empleados)
        {
            int mayor = int.MinValue;
            int posicion = 0;
            for (int contador = 0; contador < 5; contador++)
            {
                if (sueldo[contador] > mayor)
                {
                    mayor = sueldo[contador];
                    posicion = contador;
                }
            }
            Console.Clear();
            Console.WriteLine($"El empleado con el salario mayor es {empleados[posicion]}\nTiene un salario de: ${sueldo[posicion]}");

        }
    }
}
