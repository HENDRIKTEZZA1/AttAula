# AttAula 
using System;

public class Buscador
{
    public static void Main(string[] args)
    {
        string[] nomesNumeros = new string[10] {
            "15", "8", "120", "99", "50",
            "42", "7", "23", "10", "3"
        };

        string termoBusca;
        int posicaoEncontrada = -1;

        Console.WriteLine("========================================");
        Console.WriteLine("Buscador em Vetor (10 posições)");
        Console.WriteLine("========================================");
        Console.WriteLine("Digite o número que deseja buscar:");

        termoBusca = Console.ReadLine();

        for (int i = 0; i < nomesNumeros.Length; i++)
        {
            if (nomesNumeros[i] == termoBusca)
            {
                posicaoEncontrada = i;
                break;
            }
        }

        if (posicaoEncontrada != -1)
        {
            Console.WriteLine($"\nResultado: Item '{termoBusca}' encontrado na posição: {posicaoEncontrada}");
        }
        else
        {
            Console.WriteLine($"\nResultado: não encontrado");
        }
    }
}
