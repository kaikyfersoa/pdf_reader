# PDF Search Tool

Este é um script simples em Python que busca por uma palavra-chave em arquivos PDF dentro de uma determinada pasta. O script utiliza a biblioteca PyMuPDF (fitz) para manipulação de documentos PDF.

## Requisitos
- Python 3.x
- PyMuPDF (fitz)

Você pode instalar a biblioteca PyMuPDF usando o seguinte comando:
```bash
pip install PyMuPDF
```

## Como Usar
1. Execute o script.
2. Insira o caminho da pasta que contém os arquivos PDF quando solicitado.
3. Digite a palavra-chave que você deseja procurar nos arquivos PDF.

O script listará os arquivos PDF que contêm a palavra-chave e salvará os resultados em um arquivo de texto chamado `resultados_palavra-chave.txt`.

## Funções Principais

### `obter_arquivos_pdf_da_pasta(caminho_pasta)`
Esta função recebe o caminho de uma pasta como parâmetro e retorna uma lista com os nomes dos arquivos PDF presentes nessa pasta.

### `buscar_palavra_chave_no_pdf(caminho_arquivo, palavra_chave)`
Esta função recebe o caminho de um arquivo PDF e uma palavra-chave como parâmetros. Ela verifica se a palavra-chave está presente em alguma página do PDF.

### `main()`
A função principal do script:
- Solicita o caminho da pasta e a palavra-chave ao usuário.
- Lista os arquivos PDF na pasta.
- Procura a palavra-chave em cada PDF.
- Exibe os arquivos que contêm a palavra-chave.
- Salva os resultados em um arquivo de texto.

## Observações
- Certifique-se de ter a biblioteca PyMuPDF (fitz) instalada antes de executar o script.
- O script diferencia maiúsculas de minúsculas ao procurar a palavra-chave nos PDFs.
- Os resultados são salvos em um arquivo de texto para referência futura.

**Autor:** Kaiky Fernandes
