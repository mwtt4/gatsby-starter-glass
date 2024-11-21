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

**Primeiro, vamos entender o que é um LLM:**

Um LLM ou Large Language Model (Modelo de Linguagem de Grande Escala) é um sistema avançado de inteligência artificial projetado para compreender e gerar textos de forma similar à linguagem humana. Eles são os responsáveis pelas respostas elaboradas que você recebe ao interagir com eles.

**Exemplos de LLMs:**
- GPT-3 e GPT-4 da OpenAI
- BERT do Google
- LLaMA da Meta

**Características de um LLM:**
- São capazes de realizar diversas tarefas relacionadas ao processamento de linguagem natural (NLP), como geração de texto, tradução automática, respostas a perguntas, entre outras.
- Baseiam-se na arquitetura Transformer (um tipo de modelo neural) ou em variações dessa arquitetura.

![llm](/media/llm.png)


**Tá beleza, mas como os LLMs geram os textos que aparecem pra mim?**

Vamos entender como isso é feito através das etapas de pré treinamento de um LLM.

## Primeira fase - Pré Treinamento LLM: 
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

## **Fase de Tokenização:**
![token-2](/media/token-2.png)
- Tokeniza o texto de entrada do LLM na fase de pré processamento. 
- São mais gerais que palavras, lida com erro de digitação 
- Tokeniza caractere por caractere (A media de cada token tem de 3 a 4 letras)
- Permitem um equilíbrio entre a generalidade de caracteres e a eficiência de palavras.
- Cada token tem seu ID único e exclusivo, o modelo aprende com base nas palavras que estão ao redor. 

**Informações adicionais:**
- Existem vários algoritmos para codificação de tokens
- Treinar tokenizadores leva muito tempo

**Modelagem Autorregressiva:**
Os LLMs utilizam modelagem de linguagem autorregressiva, que decompõe a probabilidade de uma sequência em probabilidades condicionais para cada token, dado o contexto anterior.

![token](/media/token.png)

**Arquitetura do Modelo:**
Embora não seja o foco principal, a arquitetura do modelo (geralmente baseada em transformers) é responsável por processar os tokens de entrada e gerar representações contextuais.

## Principais pontos da fase de pré treinamento: 

- **Coleta de Dados:** Utilização de web crawlers para varrer todo o conteúdo da internet 

- **Quebra do Texto:** O computador divide todo esse texto em pedacinhos menores chamados "tokens". Esses tokens podem ser palavras inteiras, partes de palavras ou até mesmo letras individuais, conforme foi dito na parte de Tokenização

- **Aprendizado de Padrões:** O computador começa a notar padrões nesses tokens. Ele aprende que depois da palavra "o" geralmente vem um substantivo, ou que "bom" e "dia" frequentemente aparecem juntos.

- **Probabilidade:** O computador pratica tentando realizar a probabiliade da próxima palavra aparecer em uma frase. 

- **Aprendendo com Erros:** Quando o computador erra, ele ajusta seu entendimento. Se ele adivinhou uma palavra errada e colocou na frase, ele vê que não faz muito sentido e tenta melhorar na próxima vez.

- **Repetição em Grande Escala:**: Este processo é repetido bilhões de vezes com diferentes textos. Quanto mais o computador pratica, melhor ele fica em entender e prever a linguagem.

- **Desenvolvimento de Compreensão:**: Com o tempo, o computador não só aprende a prever palavras, mas também começa a entender conceitos, contextos e até mesmo algumas nuances da linguagem.

O pré-treinamento é computacionalmente intensivo, requerendo hardware especializado e otimizações de sistema.
Este processo de pré-treinamento cria um modelo base que pode ser posteriormente refinado para tarefas específicas através de técnicas como fine-tuning ou prompting.


## Segunda fase - Pós Treinamento LLM:

A segunda fase e ultima é o pós treinamento também conhecida como fine-tuning ou ajuste fino, nessa etapa você treina o modelo para dar melhores respostas baseado no que você quer que seja o objetivo dele, é aqui que o modelo vira o seu assistente IA.  

**Benefícios do Pós-treinamento:**

- **Personalização:** Adapta o modelo para domínios ou tarefas específicas.
- **Aumento da precisão:** Reduz a chance de "alucinações" do modelo.
- **Maior confiabilidade:** Melhora a qualidade e relevância das respostas.
- **Tempo de resposta reduzido:** Pode resultar em respostas mais rápidas para tarefas específicas.


**Exemplos de treinamentos de Fine-tuning:**

Métodos de Fine-tuning:
- **RLHF (Reinforcement Learning from Human Feedback):** Treinamento com feedback humano para alinhar o modelo com preferências e valores humanos
- **LoRA (Low-Rank Adaptation):** Técnica eficiente que ajusta apenas alguns parâmetros específicos do modelo
- **Instruction Tuning:** Treinamento específico com conjuntos de instruções para melhorar a capacidade de seguir comandos

Esse foi um resumo de tudo que aprendi até agora sobre LLMs, pretendo aprofundar em cada um dos tópicos e fazer posts separados sobre cada tema, aqui eu apenas mostrei o básico de como um LLM funciona por debaixo dos panos. 