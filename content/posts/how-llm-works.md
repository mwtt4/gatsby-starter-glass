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

##### Primeiro, vamos entender o que é um LLM:

Um LLM ou Large Language Model (Modelo de Linguagem de Grande Escala) é um sistema avançado de inteligência artificial projetado para compreender e gerar textos de forma similar à linguagem humana. Eles são os responsáveis pelas respostas elaboradas que você recebe ao interagir com eles.

**Exemplos de LLMs:**
- GPT-3 e GPT-4 da OpenAI
- BERT do Google
- LLaMA da Meta

**Características de um LLM:**
- São capazes de realizar diversas tarefas relacionadas ao processamento de linguagem natural (NLP), como geração de texto, tradução automática, respostas a perguntas, entre outras.
- Baseiam-se na arquitetura Transformer (um tipo de modelo neural) ou em variações dessa arquitetura.

![llm](/media/llm.png)



##### Tá beleza, mas como os LLMs geram os textos que aparecem pra mim?

Vamos entender como isso é feito através das etapas de pré treinamento de um LLM.

##### Primeira fase - Pré Treinamento LLM: 

O pré-treinamento é o alicerce de todo LLM. Nesta fase inicial, o modelo é exposto a uma quantidade massiva de textos da internet, onde aprende:
- Padrões linguísticos
- Conhecimento geral
- Estruturas gramaticais
- Contextos e relações entre palavras

**Web crawlers (robôs especializados) vasculham milhões de páginas, coletando textos de diversas fontes como:**
- Artigos científicos
- Livros digitais
- Páginas da web
- Documentações técnicas
- Fóruns de discussão

Esta fase é crucial pois estabelece a base de conhecimento que permite ao modelo compreender e gerar texto de forma coerente. É como ensinar um bebê a falar: primeiro ele precisa ser exposto a muita linguagem antes de começar a se comunicar.

##### **Fase de Tokenização:**
- Tokeniza o texto de entrada do LLM na fase de pré processamento. 
- São mais gerais que palavras, lida com erro de digitação 
- Tokeniza caractere por caractere (A media de cada token tem de 3 a 4 letras)
- Permitem um equilíbrio entre a generalidade de caracteres e a eficiência de palavras.
- Cada token tem seu ID único e exclusivo, o modelo aprende com base nas palavras que 
estão ao redor. 




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
