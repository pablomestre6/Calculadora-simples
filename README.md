# Calculadora-simples

using System;

namespace Calculator // Note: actual namespace depends on the project name.
{
    internal class Program
    {
        static void Main(string[] args)
        {
           Menu();

        }


      static void Menu()
      {
        Console.Clear();

        Console.WriteLine("O que deseja Fazer?");
        Console.WriteLine("1 - Soma");
        Console.WriteLine("2 - Subtração");
        Console.WriteLine("3 - Divisão");
        Console.WriteLine("4 - Multiplicação");
        Console.WriteLine("5 sair");
        Console.WriteLine("Obrigado por usa minha calculadora colão");

        Console.WriteLine("_ _ _ _ _ _ _");
        Console.WriteLine("Selecione uma opção");
        short res = short.Parse(Console.ReadLine());

       switch(res){
        case 1: Soma(); break;
        case 2: Subitracao(); break;
        case 3: Divisão(); break;
        case 4: Multiplicacao(); break;
        case 5: System.Environment.Exit(0); break;
        default: Menu(); break;
       

       }

      }
      
        static void Soma()
        {
            Console.Clear();
            Console.WriteLine("Primeiro Valor");
            float v1 = float.Parse(Console.ReadLine());

          Console.WriteLine("Segundo Valor");
          float v2 = float.Parse(Console.ReadLine());

            Console.WriteLine("");

          float resultado = v1 + v2;
        //  Console.WriteLine("O resultado da soma é " + resultado);
          Console.WriteLine($"O resultado da soma é {resultado}");
        //   Console.WriteLine($"O resultado da soma é {v1 + v2}");
        //   Console.WriteLine($"O resultado da soma é " + (v1 + v2));

        Console.Read();
        Menu();
        }
    
    static void Subitracao()
    {
        Console.Clear();

        Console.WriteLine("Primeiro Valor:");
        float v1 = float.Parse(Console.ReadLine());

        Console.WriteLine("Segundo  Valor:");
        float v2 = float.Parse(Console.ReadLine());

        Console.WriteLine("");

        float resultado = v1 - v2;
        Console.WriteLine($"O resultado da subtração é {resultado}");
        Console.ReadKey();
        Menu();

       }
    
    static void Divisão()
    {
        Console.Clear();

        Console.WriteLine("Primeiro valor:");
        float v1 = float.Parse(Console.ReadLine());

        Console.WriteLine("Segundo valor:");
        float v2 = float.Parse(Console.ReadLine());

        Console.WriteLine("");

        float resultado = v1/v2;
        Console.WriteLine($"O Resultado da divisão é  {resultado}");
        Console.ReadKey();
        Menu();

    }
    static void Multiplicacao()
    {
        Console.Clear();

        Console.WriteLine("Primeiro Valor");
        float v1 = float.Parse(Console.ReadLine());

        Console.WriteLine("Segundo Valor");
        float v2 = float.Parse(Console.ReadLine());

        Console.WriteLine("");

        float resultado =   v1 * v2;
        Console.WriteLine(" O resultado da multiplicação é " + (v1 * v2));
        Console.ReadKey();
        Menu();
    }

    }
}
