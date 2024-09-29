//2 questao
using System;
using System.Collections.Generic;

class Program
{
    static List<int> GenerateFibonacci(int num)
    {
        // Gera a sequência de Fibonacci até o número num
        List<int> fibList = new List<int> { 0, 1 };
        while (fibList[fibList.Count - 1] < num)
        {
            int nextValue = fibList[fibList.Count - 1] + fibList[fibList.Count - 2];
            fibList.Add(nextValue);
        }
        return fibList;
    }

    static bool IsInFibonacci(int num)
    {
        if (num < 0)
            return false;
        List<int> fibList = GenerateFibonacci(num);
        return fibList.Contains(num);
    }

    static void Main()
    {
        // Solicita um número ao usuário
        try
        {
            Console.Write("Informe um número: ");
            int inputNumber = int.Parse(Console.ReadLine());
            if (IsInFibonacci(inputNumber))
            {
                Console.WriteLine($"O número {inputNumber} pertence à sequência de Fibonacci.");
            }
            else
            {
                Console.WriteLine($"O número {inputNumber} não pertence à sequência de Fibonacci.");
            }
        }
        catch (FormatException)
        {
            Console.WriteLine("Por favor, insira um número válido.");
        }
    }
}

//3 questao 
using System;
using System.Collections.Generic;
using System.Linq;

class Program
{
    static void Main()
    {
        // Exemplo de faturamento diário em um mês (30 dias)
        List<decimal> faturamentoDiario = new List<decimal>
        {
            100, 200, 300, 150, 400, 250, 0, 300, 350, 400,
            500, 450, 200, 150, 100, 300, 600, 700, 800, 400,
            250, 300, 100, 200, 350, 400, 500, 600, 700, 800
        };

        decimal menorValor = faturamentoDiario.Min();
        decimal maiorValor = faturamentoDiario.Max();
        decimal mediaMensal = faturamentoDiario.Average();
        int diasAcimaMedia = faturamentoDiario.Count(valor => valor > mediaMensal);

        Console.WriteLine($"Menor valor de faturamento: R$ {menorValor}");
        Console.WriteLine($"Maior valor de faturamento: R$ {maiorValor}");
        Console.WriteLine($"Número de dias com faturamento acima da média: {diasAcimaMedia}");
    }
}
//4 questao
using System;
using System.Collections.Generic;

class Program
{
    static void Main()
    {
        // Faturamento mensal por estado
        Dictionary<string, decimal> faturamentoPorEstado = new Dictionary<string, decimal>
        {
            { "SP", 67836.43m },
            { "RJ", 36678.66m },
            { "MG", 29229.88m },
            { "ES", 27165.48m },
            { "Outros", 19849.53m }
        };

        // Cálculo do faturamento total
        decimal faturamentoTotal = 0;
        foreach (var valor in faturamentoPorEstado.Values)
        {
            faturamentoTotal += valor;
        }

        // Cálculo e exibição do percentual de cada estado
        Console.WriteLine("Percentual de representação por estado:");
        foreach (var estado in faturamentoPorEstado)
        {
            decimal percentual = (estado.Value / faturamentoTotal) * 100;
            Console.WriteLine($"{estado.Key}: {percentual:F2}%");
        }
    }
}
//5 
using System;

class Program
{
    static void Main()
    {
        // Entrada da string (pode ser definida diretamente ou através da entrada do usuário)
        Console.Write("Digite uma string para inverter: ");
        string entrada = Console.ReadLine();

        // Inverter a string
        string resultado = InverterString(entrada);

        // Exibir o resultado
        Console.WriteLine("String invertida: " + resultado);
    }

    static string InverterString(string s)
    {
        char[] caracteres = new char[s.Length];
        int j = 0;

        // Laço para inverter a string
        for (int i = s.Length - 1; i >= 0; i--)
        {
            caracteres[j] = s[i];
            j++;
        }

        return new string(caracteres);
    }
}

