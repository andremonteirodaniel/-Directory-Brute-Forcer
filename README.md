# -Directory-Brute-Forcer
```markdown
# 📂 DirBrute: Directory Brute-Forcer

Uma ferramenta de força bruta em Python para descobrir diretórios e arquivos ocultos ou não listados em um servidor web. Ela testa entradas de uma *wordlist* contra a URL base e reporta os códigos de status HTTP diferentes de 404 (Not Found).

## ✨ Funcionalidades

* **Força Bruta de Caminhos:** Testa uma lista de palavras para encontrar caminhos válidos no servidor.
* **Verificação de Status HTTP:** Identifica caminhos que retornam códigos de status diferentes de 404, como 200 (OK), 301 (Moved Permanently), ou 403 (Forbidden).
* **Processamento de Wordlist:** Lê um arquivo de texto contendo a lista de palavras a serem testadas.

## ⚙️ Pré-requisitos

Certifique-se de ter o Python instalado. A biblioteca `requests` é necessária.

## 📦 Instalação

1.  Clone o repositório:
    ```bash
    git clone 
    cd SeuRepositorio
    ```
2.  Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```

## 🚀 Uso

Execute o script fornecendo a URL alvo e o caminho para o arquivo da *wordlist* como argumentos.

```bash
python dirbrute.py <URL_ALVO> <CAMINHO_WORDLIST>
# Exemplo: python dirbrute.py [http://exemplo.com](http://exemplo.com) /caminho/para/wordlist.txt
