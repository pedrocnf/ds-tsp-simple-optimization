# ds-tsp-simple-optimization
Aplicação do algoritmo do caixeiro viajante com abordagem genética para solução de um problema de roteirização

# Resolvendo o Problema do Caixeiro Viajante (TSP) com Algoritmos Genéticos

Este é um guia de implementação para resolver o Problema do Caixeiro Viajante (TSP) usando Algoritmos Genéticos em Python. Este README fornece uma visão geral detalhada e instruções para aplicar conceitos de otimização e algoritmos genéticos em problemas de roteamento.

## Sumário

- [Introdução ao TSP](#introdução-ao-tsp)
- [Algoritmos Genéticos e o TSP](#algoritmos-genéticos-e-o-tsp)
- [Implementação em Python](#implementação-em-python)
  - [Pré-Requisitos](#pré-requisitos)
  - [Código-Base](#código-base)
- [Conclusão](#conclusão)

## Introdução ao TSP

O Problema do Caixeiro Viajante (TSP) é um problema clássico em otimização que envolve encontrar a rota mais curta para visitar um conjunto de cidades e retornar à cidade de origem. É um problema NP-Difícil, significando que encontrar a solução ótima pode ser extremamente desafiador, especialmente para instâncias com muitas cidades.

## Algoritmos Genéticos e o TSP

Algoritmos Genéticos são uma família de algoritmos de busca e otimização baseados nos processos de seleção natural e genética. Eles são especialmente úteis para resolver problemas complexos como o TSP, onde o espaço de soluções é grande e as soluções ótimas são difíceis de encontrar.

### Conceitos-chave dos AGs:

- **População**: Conjunto de soluções candidatas.
- **Fitness**: Métrica que avalia a qualidade de uma solução.
- **Seleção**: Processo de escolha de soluções para reprodução.
- **Crossover**: Combinação de duas soluções para criar uma nova.
- **Mutação**: Introdução de variações aleatórias nas soluções.
- **Geração Nova**: Substituição da população atual pela nova geração após o crossover e a mutação.

## Implementação em Python

### Pré-Requisitos

- Python 3.x
- Bibliotecas: DEAP, Pandas, Matplotlib
- Instale as bibliotecas com `pip install deap pandas matplotlib`

### Código-Base

1. **Configuração Inicial e Matriz de Distâncias**

   Definimos a matriz de distâncias entre as cidades. Em um cenário real, esta matriz pode ser derivada de dados geográficos.

   ```python
   import pandas as pd
   # Exemplo de matriz de distâncias
   data = {...}  # Substitua com sua matriz
   distance_matrix = pd.DataFrame(data)

