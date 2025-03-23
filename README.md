# AI-Assisted Research with LLMs

Este projeto demonstra como usar APIs de **LLMs (Large Language Models)**, como o **Tavily** e o **Exa.ai**, junto com o modelo **Ollama** para realizar pesquisas inteligentes e gerar resumos. Este é um exemplo básico de uso, que pode ser facilmente integrado a projetos de **RAG** (Retrieval-Augmented Generation) ou **AI Agents**, oferecendo a capacidade de adicionar contexto ou obter conteúdos da internet.

## Features

- **Pesquisa de Informações**: Realiza buscas sobre um nome de pessoa usando as APIs **Tavily** e **Exa.ai**.
- **Geração de Resumo**: Utiliza o modelo **Ollama** (LLama 3.2) para resumir o conteúdo obtido das buscas.
- **Integração com AI Agents**: Pode ser integrado a sistemas de RAG ou AI Agents para criar fluxos mais complexos com contexto dinâmico.

## Getting Started

### Prerequisites

- Python 3.7 ou superior
- Pacotes Python necessários (veja `requirements.txt`)
- **Ollama** (para uso do modelo `llama3.2:1b`)
- Tavily API e Exa.ai API

### Instalação

1. Clone o repositório:

   ```bash
   git clone https://github.com/seu_usuario/nome_do_repositorio.git
   cd nome_do_repositorio

2. Crie um ambiente virtual (opcional, mas recomendado):

    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows: venv\Scripts\activate

3. Instale as dependências:

    ```bash
    pip install -r requirements.txt

4. Instalar o Ollama:
    ```bash
    ollama pull llama3.2:1b

5. Configurar o arquivo .env:
    ```bash
    TAVILY_API_KEY=SuaChaveTavilyAqui
    EXA_API_KEY=SuaChaveExaAqui

### Uso

1. Execute o notebook llm_research.ipynb:

2. O notebook solicitará que você digite algo a ser pesquisado. Ele irá:
    - Buscar informações utilizando Tavily e Exa.ai.
    - Gerar um resumo usando o modelo LLM llama3.2:1b com Ollama.