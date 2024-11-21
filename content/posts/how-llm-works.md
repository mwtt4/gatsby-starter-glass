---
title: Como funcionam os LLMs?
date: 2024-11-20
tags:
  - Machine Learning
  - IA
  - "2024"
social_image: /media/llm.png
description: Esse artigo mergulha no fascinante mundo dos LLMs (Large Language Models), revelando como modelos como o ChatGPT funcionam nos bastidores. Descubra a arquitetura por trás dessas IAs, entenda como elas geram textos tão coerentes e explore o processo que permite que elas acessem e processem informações de forma tão eficiente
---

Após o meu primeiro contato com o ChatGPT, fiquei impressionado com a rapidez com que esse modelo de linguagem (LLM) responde às perguntas. Isso despertou em mim algumas dúvidas: Como ele funciona nos bastidores? Qual é sua arquitetura? Como o ChatGPT consegue fornecer respostas para as minhas perguntas? Como ele gera esses textos? E a partir de que base?

Com essas questões em mente, decidi me aprofundar no estudo e na pesquisa sobre o funcionamento dos LLMs. Neste artigo, compartilho tudo o que aprendi ao longo dessa jornada.

### Primeiro, vamos entender o que é um LLM:

Um LLM ou Large Language Model (Modelo de Linguagem de Grande Escala) é um sistema avançado de inteligência artificial projetado para compreender e gerar textos de forma similar à linguagem humana. Eles são os responsáveis pelas respostas elaboradas que você recebe ao interagir com eles.

Exemplos de LLMs:
- GPT-3 e GPT-4 da OpenAI
- BERT do Google
- LLaMA da Meta

![llm](/media/llm.png)

Características de um LLM: 
- São capazes de realizar diversas tarefas relacionadas ao processamento de linguagem natural (NLP), como geração de texto, tradução automática, respostas a perguntas, entre outras.
- Baseiam-se na arquitetura Transformer (um tipo de modelo neural) ou em variações dessa arquitetura.



### Tá beleza, mas como os LLMs geram os textos que aparecem pra mim?

Vamos entender como isso é feito através das etapas de pré treinamento de um LLM.

Primeira fase - Pré Treinamento LLM: 

O pré-treinamento é o alicerce de todo LLM. Nesta fase inicial, o modelo é exposto a uma quantidade massiva de textos da internet, onde aprende:
- Padrões linguísticos
- Conhecimento geral
- Estruturas gramaticais
- Contextos e relações entre palavras

## Unordered Lists

- Item 1
- Item 2
- Item 3

## Ordered Lists

1. Item 1
2. Item 2
3. Item 3

## Code Block

```javascript
// finds a given word in a string and replace with another one
const findAndReplace = (string, wordToFind, wordToReplace) => {
  return string.split(wordToFind).join(wordToReplace);
};

let result = findAndReplace('I like banana', 'banana', 'apple'); // I like apple
```

## Quoted Text

> Maecenas faucibus mollis interdum. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Aenean lacinia bibendum nulla sed consectetur. Etiam porta sem malesuada magna mollis euismod. Donec sed odio dui. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla vitae elit libero, a pharetra augue.
