# Extrator de Conteúdo de Sitemap

Este script em Python extrai o conteúdo textual de páginas listadas em um sitemap XML e gera um documento do Word (`.docx`) com o conteúdo extraído. Ele utiliza `requests`, `BeautifulSoup` e `python-docx` para raspagem de dados e criação de documentos.

## Funcionalidades

- Faz o parsing de um sitemap XML para extrair URLs.
- Realiza a raspagem de conteúdo textual de cada página.
- Remove elementos desnecessários como `<script>` e `<style>`.
- Gera um documento Word limpo e estruturado com títulos para cada URL.

## Requisitos

Você pode instalar todas as dependências com o seguinte comando:

```bash
pip install -r requirements.txt
```

## Como Usar

1. Clone este repositório ou baixe o script.
2. Instale as dependências necessárias utilizando o comando acima.
3. Atualize a variável sitemap_url no script com a URL do sitemap desejado.
4. Execute o script:

   ```bash
   python app.py
   ```

## Estrutura de Arquivos

```
.
├── app.py                  # Script principal em Python
├── requirements.txt        # Lista de dependências
└── site_content.docx       # Documento Word gerado com o conteúdo extraído
```

## Exemplo

Para utilizar o script com o sitemap http://example.com/sitemap.xml, atualize a seguinte linha no código:

```python
sitemap_url = 'http://example.com/sitemap.xml'
```

Após executar o script, o conteúdo extraído será salvo no arquivo  `site_content.docx`.

## Observações

- Certifique-se de que o sitemap XML esteja acessível e siga o formato padrão.
- Sitemaps muito grandes podem levar mais tempo para serem processados.
