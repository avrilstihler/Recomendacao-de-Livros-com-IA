# 📚✨ Seu Guia Literário Pessoal com IA Gemini ✨📚

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/avrilstihler/Recomendacao-de-Livros-com-IA/blob/main/sistema_recomendacao_livros_gemini.ipynb)

Cansado de não saber o que ler em seguida? Quer descobrir se aquele livro famoso é realmente para você? Este projeto utiliza o poder do Google Gemini e do Google Agent Development Kit (ADK) para criar um **Sistema de Descoberta e Recomendação Literária** inteligente e interativo!

Nossos agentes de IA trabalham juntos para te ajudar a:
*   🔎 **Analisar um livro específico:** Descubra se vale a pena a leitura com um perfil detalhado.
*   💡 **Encontrar livros similares:** Amou um livro? Encontre outros com a mesma vibe, tema ou estilo!
*   🗺️ **Explorar por temas:** Buscando algo sobre aventura, romance, mistério ou filosofia? Nós te ajudamos!

---

## 🎯 Objetivo Principal

Facilitar a jornada do leitor na descoberta de novos livros e na tomada de decisão sobre qual obra explorar, oferecendo análises e recomendações personalizadas através de um sistema colaborativo de agentes de Inteligência Artificial.

---

## 🤖 Nossos Agentes Literários Especializados

O sistema é orquestrado por três agentes principais, cada um com uma missão única:

1.  **Agente Detetive Literário (`BookProfilerAgent`) 🕵️‍♂️📖:**
    *   **Missão:** Investigar a fundo um livro específico.
    *   **Habilidades:** Cria um perfil detalhado do livro, incluindo sinopse (sem spoilers!), temas centrais, estilo de escrita, tom, sentimento/vibe que transmite, público-alvo comum, pontos fortes e possíveis ressalvas.
    *   **Ferramenta Principal:** `google_search` para vasculhar resenhas, análises e discussões.

2.  **Agente Conector de Histórias (`SimilarityAnalyzerAgent`) 🔗📚:**
    *   **Missão:** Encontrar os elos perdidos entre livros e ideias.
    *   **Habilidades:**
        *   Identifica de 3 a 5 livros similares a um **livro de referência** que você amou, baseando-se em temas, estilo, tom, sentimento ou complexidade.
        *   Busca livros relevantes a um **tema ou gênero de interesse** que você fornecer.
    *   **Ferramenta Principal:** `google_search` para descobrir conexões e obras relacionadas.

3.  **Agente Curador de Recomendações (`RecommendationGeneratorAgent`) 큐레이터✨:**
    *   **Missão:** Transformar dados brutos em conselhos literários preciosos.
    *   **Habilidades:**
        *   Apresenta o perfil do livro (do Agente Detetive) de forma clara, ajudando você a decidir se deve lê-lo.
        *   Monta uma lista de recomendações atraente e convincente (do Agente Conector), explicando o porquê de cada sugestão.
    *   **Personalização:** Leva em conta seu perfil de leitor (opcional) para refinar as sugestões.

---

## ✨ Funcionalidades em Destaque

*   **Múltiplos Caminhos de Descoberta:** Escolha como quer começar sua busca: analisando um livro, buscando por similaridade ou explorando um tema.
*   **Perfil do Leitor (Opcional):** Forneça seus gostos para recomendações ainda mais alinhadas com você!
*   **Análise Detalhada de Livros:** Vá além da capa com insights sobre temas, estilo e o "sentimento" da obra.
*   **Recomendações Inteligentes:** Descubra livros que realmente combinam com o que você procura.
*   **Interação Amigável:** Um sistema guiado por perguntas para facilitar sua experiência.

---

## 🛠️ Tecnologias Utilizadas

*   Python 🐍
*   Google Gemini API (`google-genai`) - Modelo `gemini-2.0-flash` (ou outro)
*   Google Agent Development Kit (`google-adk`)
*   Google Search (como ferramenta dos agentes)
*   Google Colaboratory (ambiente de execução)

---

## 🚀 Como Começar sua Aventura Literária

1.  **API Key Mágica 🔑:** Você precisará de uma API Key do Google Gemini. Obtenha a sua no [Google AI Studio](https://aistudio.google.com/app/apikey).
2.  **Abra o Portal no Colab:** Clique no botão "Open In Colab" no topo deste README.
3.  **Guarde o Segredo 🤫:** No Colab, vá em "Secrets" (ícone de chave 🔑 na barra lateral) e adicione sua `GOOGLE_API_KEY`.
4.  **Desperte os Agentes ▶️:** Execute as células do notebook em ordem.
5.  **Converse com o Sistema 🗣️:** Responda às perguntas para guiar os agentes. Você pode:
    *   Pedir uma investigação sobre um livro.
    *   Solicitar recomendações baseadas em um livro que você já ama.
    *   Explorar livros por um tema ou gênero específico.
6.  **Receba suas Descobertas 🎁:** Veja os relatórios e listas de recomendações criados especialmente para você!

---

Prepare-se para encontrar sua próxima leitura favorita! Este sistema é uma demonstração de como a IA pode ser uma companheira incrível na exploração do vasto universo dos livros. Experimente, adapte e boa leitura! 🌟
