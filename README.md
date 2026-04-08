# Práticas: Simulações Estatísticas em Python

## Visão Geral

Este repositório contém duas atividades práticas que demonstram conceitos fundamentais de estatística e probabilidade através de simulações em Python:

1. **Lançamento de Moedas** - Demonstração da Lei dos Grandes Números e convergência de probabilidades
2. **Controle de Qualidade e Manutenção Preditiva** - Aplicação da Lei dos Grandes Números, Teorema Central do Limite e Teorema de Bayes


## Atividade 1: Lançamento de Moedas

### Objetivo

Demonstrar a **Lei dos Grandes Números (LGN)** através da simulação de lançamentos de uma moeda justa (probabilidade de Cara = 0.5).

### Cenário

- Moeda justa (Cara = 0.5, Coroa = 0.5)
- Lançamentos sucessivos
- Observação da convergência da proporção de Caras

### O que foi feito

| Etapa | Descrição |
| **Simulação** | Lançamentos de 10, 100, 1.000 e 10.000 vezes |
| **LGN** | Cálculo da proporção de "Caras" para cada série |
| **Gráfico** | Convergência da proporção para 0.5 |
| **Comparação** | Probabilidade observada vs teórica (10.000 lançamentos) |

### Principais Aprendizados

- Com poucos lançamentos (n=10), a proporção pode variar muito (30% a 80%)
- Conforme o número de lançamentos aumenta, a proporção se aproxima de 50%
- Com 10.000 lançamentos, o erro geralmente é menor que 1%
- A Lei dos Grandes Números garante a convergência, mas não elimina a variabilidade em amostras pequenas

## Atividade 2: Controle de Qualidade e Manutenção Preditiva

### Objetivo

Consolidar três conceitos estatísticos fundamentais através de um cenário realista de controle de qualidade industrial.

### Cenário

- **Fábrica de componentes eletrônicos**
- Taxa histórica de defeitos: **5%**
- Sensor de anomalia: sensibilidade **90%** (detecta 90% dos defeitos)
- Falso positivo: **8%** (alarme em componente bom)
- Peso dos componentes: distribuição **uniforme** (10g a 12g)

### O que foi feito

#### 1. Lei dos Grandes Números (LGN)

**Objetivo:** Demonstrar que a taxa observada de defeitos converge para a taxa teórica de 5%.

**Implementação:**
- Simulação da produção de 10, 100, 1.000 e 10.000 componentes
- Cálculo da taxa observada de defeitos em cada simulação
- Gráfico mostrando a convergência para 5%

**Resultado:**
- Com 10 componentes: taxa entre 0% e 20%
- Com 100 componentes: taxa entre 2% e 8%
- Com 1.000 componentes: taxa entre 4% e 6%
- Com 10.000 componentes: taxa muito próxima de 5%

#### 2. Teorema Central do Limite (TCL)

**Objetivo:** Demonstrar que médias amostrais de uma população não-normal seguem distribuição normal.

#### 3. Teorema de Bayes

**Objetivo:** Calcular a probabilidade real de um componente ser defeituoso dado que o sensor detectou anomalia.

## Principais Aprendizados

### Lei dos Grandes Números
- Com poucas amostras, há grande variação
- Com muitas amostras, a proporção converge para o valor teórico
- A convergência é garantida, mas não é instantânea

### Teorema Central do Limite
- A normalidade das médias amostrais independe da distribuição original
- População uniforme (não-normal) → médias amostrais normais
- O TCL é a base de muitos testes estatísticos

### Teorema de Bayes
- A intuição humana falha em problemas probabilísticos
- O cálculo formal é essencial para decisões corretas
- Falsos positivos são especialmente problemáticos quando a condição é rara

## Autora 
Letícia Moura @leletcode
