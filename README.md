# Gerador de conteúdo para marketing

Aplicação em Streamlit que usa um modelo da Groq para gerar textos de marketing com opções de plataforma, tom, tamanho, público-alvo, chamada para ação, hashtags e palavras-chave de SEO.

## Requisitos

- Python 3.10 ou superior
- Uma chave de API da Groq

## Configuração no Windows

Abra o PowerShell na pasta do projeto e crie um ambiente virtual:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

Instale as dependências:

```powershell
python -m pip install streamlit langchain-groq langchain-core python-dotenv
```

Copie o arquivo de exemplo para criar seu arquivo local de configuração:

```powershell
Copy-Item .env.example .env
```

Edite `.env` e substitua o valor de exemplo pela sua chave:

```text
GROQ_API_KEY=sua_chave_da_groq
```

## Executar

```powershell
streamlit run app.py
```

O Streamlit mostrará o endereço local da aplicação no terminal.

## Segurança

Não publique nem compartilhe o arquivo `.env` ou sua chave de API. O `.gitignore` exclui `.env` e dependências locais do GitHub; `.env.example` é apenas um modelo, sem uma chave válida. Se uma chave real for exposta, revogue-a e gere outra.
