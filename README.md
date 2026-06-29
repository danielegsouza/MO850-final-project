# MO850: Busca Semântica no Contexto de Desinformação Vacinal

Repositório do projeto final da disciplina MO850 (Tópicos Avançados em Ciência da Computação / NLP) - Instituto de Computação, Unicamp.

Este projeto explora o uso de técnicas de Processamento de Linguagem Natural (NLP) e busca semântica (SBERT) para a identificação, análise e monitoramento de narrativas de desinformação vacinal em canais do Telegram.

## Estrutura do Repositório

- `/notebooks`: Contém os cadernos interativos (Jupyter Notebooks) com todo o pipeline de extração de dados, limpeza, modelagem e avaliação, divididos por etapas (exploração, topic modeling, busca semântica e avaliação com LLMs).
- `/relatorio`: Arquivos LaTeX (\texttt{main.tex}, bibliografia, e imagens) referentes ao artigo e relatório técnico do projeto.

## Principais Contribuições e Etapas

1. **Modelagem de Tópicos (BERTopic):** Clusterização não supervisionada das mensagens com HDBSCAN + c-TF-IDF.
2. **Busca Semântica vs Léxica:** Comparação de performance utilizando embeddings contextuais versus busca por palavras-chave em 5 narrativas predefinidas.
3. **Validação Zero-Shot de Modelos de Linguagem:** Benchmark comparativo (Llama 3 8B, Llama 3.1 8B, Gemma 2 27B) e análise das fragilidades (\textit{Zero-Shot Positive Bias}).
4. **Análise de Engajamento e Viralização:** Correlação estatística entre métricas puramente semânticas (\textit{cosine similarity}) e métricas de engajamento do mundo real (forwards e visualizações).

## Tecnologias e Bibliotecas Utilizadas
- **Python 3.12+**
- **HuggingFace Transformers e Sentence-Transformers**
- **BERTopic**, **UMAP**, **HDBSCAN**
- **Pandas, Seaborn, Matplotlib, SciPy**

## Autor
Daniele Souza Gonçalves
(d248029@dac.unicamp.br)
