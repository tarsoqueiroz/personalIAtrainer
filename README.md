# Assistente de Personal Trainer - Gerador de Treino Ideal

Este projeto é um desafio de Prompt Engineer, onde o objetivo é criar um prompt que ajuda a montar o treino ideal para cada combinação de fatores, como biotipo corporal, disponibilidade de tempo e tipo de exercícios preferidos. O assistente de personal trainer gerado por esse prompt será capaz de personalizar os treinos de acordo com as características e necessidades do usuário. O projeto deve ser feito utilizando as boas práticas de prompt engineer.

## Índice

- [Assistente de Personal Trainer - Gerador de Treino Ideal](#assistente-de-personal-trainer---gerador-de-treino-ideal)
  - [Índice](#índice)
  - [Objetivo](#objetivo)
  - [Biotipos Corporais](#biotipos-corporais)
  - [Dias Disponíveis para Treino](#dias-disponíveis-para-treino)
  - [Tipos de Exercícios](#tipos-de-exercícios)
  - [Regras de negócio](#regras-de-negócio)
  - [Desenvolvimento da Proposta de Prompt](#desenvolvimento-da-proposta-de-prompt)
  - [Prompt de Resposta Proposto](#prompt-de-resposta-proposto)

## Objetivo

Este projeto é um desafio de Prompt Engineer, onde o objetivo é criar um prompt que ajuda a montar o treino ideal para cada combinação de fatores, como biotipo corporal, disponibilidade de tempo e tipo de exercícios preferidos. O assistente de personal trainer gerado por esse prompt será capaz de personalizar os treinos de acordo com as características e necessidades do usuário.

O projeto deve ser feito utilizando as boas práticas de prompt engineer.

## Biotipos Corporais

A primeira regra para personalizar o treino é determinar o biotipo corporal do usuário. Existem três biotipos principais:

| Imagem | Biotipo | Descrição |
| :----- | :------ | :-------- |
| ![Ectomorfo](./images/ectomorph.jpg) | **Ectomorfo** | Corpo mais magro, difícil ganhar peso e massa muscular. |
| ![Mesomorfo](./images/mesomorph.jpg) | **Mesomorfo** | Corpo naturalmente musculoso, facilidade para ganhar massa muscular e perder gordura. |
| ![Endomorfo](./images/endmorph.jpg)  | **Endomorfo** | Corpo com tendência a acumular gordura, maior dificuldade em perder peso. |

> **Nota:** Escolha o biotipo que mais se aproxima do seu corpo atual para que o treino seja mais eficiente.

## Dias Disponíveis para Treino

A segunda regra é determinar quantos dias por semana o usuário tem disponível para treinar. Dependendo do número de dias, o treino sugerido pode variar:

| **Dias por Semana** | **Tipo de Treino Sugerido** | **Detalhamento do Treino** |
| :-----------------: | --------------------------- | -------------------------- | 
| 1 dia               | Treino Full Body            | Treino que trabalha o corpo todo em uma única sessão. |
| 3 dias              | Treino ABC                  | Divisão do treino em três dias, cada um focado em grupos musculares diferentes. |
| 5 dias              | Treino ABCDE                | Divisão do treino em cinco dias, com foco ainda mais específico em cada grupo muscular. |

## Tipos de Exercícios

A terceira regra envolve a escolha do tipo de exercício preferido. Aqui estão algumas categorias com exemplos:

| **Imagem**                          | **Tipo de Treino** | **Descrição**                                                                                                 |
| ----------------------------------- | ------------------ | ------------------------------------------------------------------------------------------------------------- |
| ![Funcional](./images/dumbells.png) | **Funcional**      | Exercícios que melhoram a funcionalidade do corpo, usando movimentos naturais.                                |
| ![Maquinario](./images/4760665.png) | **Maquinário**     | Exercícios feitos em máquinas, com foco em isolar grupos musculares.                                          |
| ![Peso Livre](./images/barr.png)    | **Peso Livre**     | Exercícios com pesos livres, como halteres e barras, para trabalhar vários grupos musculares simultaneamente. |
| ![Cardio](./images/cardio.png)      | **Cardio**         | Exercícios voltados para melhorar a resistência cardiovascular, como corrida ou ciclismo.                     |
| ![HIIT](./images/hiit.png)          | **HIIT**           | Treinos intervalados de alta intensidade, ótimos para queima de gordura.                                      |

## Regras de negócio

1. **Identifique seu biotipo corporal** consultando a seção de biotipos.
1. **Determine quantos dias por semana você pode treinar** e escolha o tipo de treino mais adequado.
1. **Selecione o tipo de exercício** que prefere realizar e que se encaixa melhor nos seus objetivos.
1. Use o prompt do assistente para gerar um plano de treino personalizado.

## Desenvolvimento da Proposta de Prompt

Considerando as informações a serem obtidas para preencher a regra de negócio (biotipo corporal, disponibilidade de tempo e tipo de exercícios preferidos), adiciona-se ainda as seguintes questões para melhor identificar o cliente:

- **Nome**: informação para identificar/personalizar a proposta;
- **Sexo**: orientar os tipos de exercício;
- **Idade**: calibrar a carga e tempo dos exercícios.

## Prompt de Resposta Proposto

Com base no desenvolvimento anterior, o questionário de identificação e avaliação do cliente irá obter as seguintes informações a serem utilizadas no prompt:

- Nome
- Idade
- Sexo
- Biotipo
- Disponibilidade em dias por semana
- Categoria de exercícios

Propõe-se o seguinte prompt informando os dados acima coletados para produzir as atividades em cada sessão:

***Vamos criar um plano de treinamento individualizado.***

Considerando os seguintes biotipos corporais:

1) Ectomorfo: Corpo mais magro, difícil ganhar peso e massa muscular.
2) Mesomorfo: Corpo naturalmente musculoso, facilidade para ganhar massa muscular e perder gordura.
3) Endomorfo: Corpo com tendência a acumular gordura, maior dificuldade em perder peso.

Considerando também os seguintes tipos de treino com base na disponibilidade de dias:

1) 1 dia por semana: Treino Full Body que trabalha o corpo todo em uma única sessão.
2) 3 dias por semana: Treino ABC que divide o treino em três dias, cada um focado em grupos musculares diferentes.
3) 5 dias por semana: Treino ABCDE que divide o treino em cinco dias, com foco ainda mais específico em cada grupo muscular.

Finalmente, considerando o exercício preferido do cliente em uma ou mais das seguintes categorias:

1) Funcional: Exercícios que melhoram a funcionalidade do corpo, usando movimentos naturais.
2) Maquinário: Exercícios feitos em máquinas, com foco em isolar grupos musculares.
3) Peso Livre: Exercícios com pesos livres, como halteres e barras, para trabalhar vários grupos musculares simultaneamente.
4) Cardio: Exercícios voltados para melhorar a resistência cardiovascular, como corrida ou ciclismo.
5) HIIT: Treinos intervalados de alta intensidade, ótimos para queima de gordura.

Assim, monte um plano de treinamento com aquecimento, especificando os exercicios, repetições e tempo, e também alongamento final para:

- Nome: "**NOME DO CLIENTE**"
- Idade: "**IDADE DO CLIENTE EM ANOS**"
- Sexo: "**SEXO DO CLIENTE**"
  - Masculino, ou
  - Feminino
- Biotipo (1 das opções): "**BIOTIPO DO CLIENTE**"
  - Ectomorfo, ou
  - Mesomorfo, ou
  - Endomorfo
- Disponibilidade em dias por semana (1 das opções): "**DISPONIBILIDAE EM DIAS NA SEMANA**"
  - 1, ou
  - 3, ou
  - 5
- Categoria de exercícios (todas as opções que se aplicam): "**QUAIS TIPOS DE EXERCÍCIOS PREFERE**"
  - Funcional, e/ou
  - Maquinário, e/ou
  - Peso Livre, e/ou
  - Cardio, e/ou
  - HIIT
