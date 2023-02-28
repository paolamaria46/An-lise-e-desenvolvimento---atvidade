# An-lise-e-desenvolvimento---atvidade

2 Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores.


num = int(input("Digite um número: "))
fib = [0, 1]

while fib[-1] < num:
    fib.append(fib[-1] + fib[-2])

if num in fib:
    printf("O número {num} pertence à sequência de Fibonacci!")
else:
    printf("O número {num} não pertence à sequência de Fibonacci.")

3 Dado um vetor que guarda o valor de faturamento diário de uma distribuidora, faça um programa, na linguagem que desejar, que calcule e retorne:

import json

with open('faturamento.json') as file:
    faturamento = json.load(file)

media_mensal = sum(faturamento.values()) / len(faturamento)
dias_acima_media = sum(1 for f in faturamento.values() if f > media_mensal)

printf("Menor valor de faturamento diário: {min(faturamento.values())}")
printf("Maior valor de faturamento diário: {max(faturamento.values())}")
printf("Número de dias com faturamento acima da média mensal: {dias_acima_media}")



4 Dado o valor de faturamento mensal de uma distribuidora, detalhado por estado:


// Valores de faturamento mensal por estado
faturamento = {"SP": 67836.43, "RJ": 36678.66, "MG": 29229.88, "ES": 27165.48, "Outros": 19849.53}

# Cálculo do total mensal de faturamento
total = sum(faturamento.values())

// Cálculo do percentual de representação de cada estado
percentuais = {}
for estado, valor in faturamento.items():
    percentuais[estado] = (valor / total) * 100

// Impressão dos resultados
for estado, percentual in percentuais.items():
    printf{“estado}: {percentual:.2f}%")



5 Escreva um programa que inverta os caracteres de um string.

// String a ser invertida
string = "Atividade"

// Inicialização da string invertida
string_invertida = ""

// Inversão dos caracteres
for i in range(len(string)-1, -1, -1):
    string_invertida += string[i]

# Impressão da string invertida
print(string_invertida)
