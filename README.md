# Projeto Prático de PLN (2026-Q3, UFABC)

Projeto da disciplina **Processamento de Linguagem Natural**, com o Prof. Alexandre Donizeti Alves.

## Equipe

- Guilherme Araujo dos Santos (RA 11202020294)
- Ian Victor Toniolo Silva (RA 11202020351)

## Ideia

O usuário informa um tema. O notebook busca o artigo correspondente na **Wikipédia em português** pela **MediaWiki Action API** e usa **LangChain + Claude Haiku 5.5** para aplicar três técnicas de PLN:

1. **Sumarização de Textos**: resumo do artigo em tópicos.
2. **Reconhecimento de Entidades Nomeadas**: pessoas, organizações, locais e datas, com saída estruturada (Pydantic).
3. **Sistema de Perguntas e Respostas**: respostas baseadas só no artigo recuperado (RAG simples).

## Tecnologias

| Item | Escolha |
|---|---|
| Framework | [LangChain](https://python.langchain.com) (`langchain-anthropic`) |
| LLM | Claude Haiku 5.5 (`claude-haiku-5-5`), [documentação](https://docs.claude.com/en/docs/about-claude/models/overview) |
| API | MediaWiki Action API, [documentação](https://www.mediawiki.org/wiki/API:Main_page) |

## Como executar

1. Abra `PLN_Projeto_Wikipedia_Claude.ipynb` no Google Colab.
2. Em **Secrets** (ícone 🔑), crie `ANTHROPIC_API_KEY` com sua chave do Claude Console.
3. Execute todas as células (*Ambiente de execução → Executar tudo*).
