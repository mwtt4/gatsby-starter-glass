---
title: Como funcionam os LLMs?
date: 2024-11-20
tags:
  - Machine Learning
  - IA
  - "2024"
social_image: /media/rocket.jpg
description: Esse artigo mergulha no fascinante mundo dos LLMs (Large Language Models), revelando como modelos como o ChatGPT funcionam nos bastidores. Descubra a arquitetura por trás dessas IAs, entenda como elas geram textos tão coerentes e explore o processo que permite que elas acessem e processem informações de forma tão eficiente
---

Após o meu primeiro contato com o ChatGPT, fiquei impressionado com a rapidez com que esse modelo de linguagem (LLM) responde às perguntas. Isso despertou em mim algumas dúvidas: Como ele funciona nos bastidores? Qual é sua arquitetura? Como o ChatGPT consegue fornecer respostas para as minhas perguntas? Como ele gera esses textos? E a partir de que base?

Com essas questões em mente, decidi me aprofundar no estudo e na pesquisa sobre o funcionamento dos LLMs. Neste artigo, compartilho tudo o que aprendi ao longo dessa jornada.

Primeiro, vamos entender o que é um LLM:

Um LLM ou Large Language Model (Modelo de Linguagem de Grande Escala) é um sistema avançado de inteligência artificial projetado para compreender e gerar textos de forma similar à linguagem humana. Eles são os responsáveis pelas respostas elaboradas que você recebe ao interagir com eles.

Exemplos de LLMs
- GPT-3 e GPT-4 da OpenAI
- BERT do Google
- LLaMA da Meta

Características de um LLM: 
- São capazes de realizar diversas tarefas relacionadas ao processamento de linguagem natural (NLP), como geração de texto, tradução automática, respostas a perguntas, entre outras.
- Baseiam-se na arquitetura Transformer (um tipo de modelo neural) ou em variações dessa arquitetura.

So, Jonathan, how was the pull-out? Hey kiddo, would you like a balloon? We never would've upset you if we knew you had superpowers. Do you know anything about sensory deprivation tanks? Specifically how to build one?Why do we even need weapons anyway? We have her. She shut one door! With her mind! I need my paddles! Mistakes have been made. We never would've upset you if we knew you had superpowers. Nobody normal ever accomplished anything meaningful in this world.Why’s he gotta kick the door? Do you know anything about sensory deprivation tanks? Specifically how to build one? I need my paddles! It’s finger-lickin’ good. You’re pretty cute, you know that? It’s finger-lickin’ good. Don’t take it so personally, okay? I don’t like most people. He’s in the vast majority.

## Image

![Rocket launch](/media/rocket.jpg)

## Header

Solebat cetera infelix duorum gravidi possit, et nec, est inpia mentique, consistere quae. Amplexus uror, pars pars aevo curas Cinyreius
pennis sacrum inpulsaque o cunctos Oleniden peragit, se Athamas inmaduit
transierant. Relicta significat rubenti potest.

Illa tibi cruentum adpulit pallent. Una dolorem quaque. Pars parvi, mihi quae
Lyciaeque legit. Hic vitae felix illi laudatis? Et caelum, precatur nec pectora,
Phoebi volucris moveo.

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
