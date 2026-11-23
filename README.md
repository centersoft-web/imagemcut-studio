# ImgForge — Conversor de Imagens

**ImgForge** é uma ferramenta web em português para conversão e redimensionamento em massa de imagens diretamente no navegador.

O processamento acontece localmente com a API Canvas do navegador. As imagens selecionadas não são enviadas para nenhum servidor.

## Recursos

- Upload de várias imagens por seletor de arquivos ou arrastar e soltar
- Exportação para **PNG, JPEG, WebP e AVIF**
- Conversão em lote
- Tamanhos predefinidos e dimensões personalizadas
- Modos de dimensionamento:
  - largura fixa, mantendo a proporção
  - altura fixa, mantendo a proporção
  - ajustar dentro das dimensões
  - preencher e cortar
- Ajuste de qualidade
- Remoção de fundo por cor
- Seleção da cor diretamente na prévia
- Controle de tolerância, suavização e nitidez
- Remoção de fundo conectado apenas às bordas
- Visualização dos resultados
- Download individual ou de todos os arquivos em um `.zip`

## Formatos suportados

Entrada: PNG, JPEG, WebP, GIF, BMP e AVIF, conforme suporte do navegador.

Saída: PNG, JPEG, WebP e AVIF, conforme suporte do navegador.

Ao ativar a remoção de fundo, PNG, WebP e AVIF preservam a transparência. Para JPEG, a área removida recebe a cor selecionada.

## Como usar

1. Abra o `index.html` em um navegador moderno ou publique a página no GitHub Pages.
2. Selecione ou arraste uma ou mais imagens.
3. Escolha um ou mais formatos de saída.
4. Escolha um ou mais tamanhos predefinidos ou configure um tamanho personalizado.
5. Ajuste a qualidade e, opcionalmente, a remoção de fundo.
6. Clique em **Processar imagens**.
7. Baixe as imagens individualmente ou use **Baixar tudo (.zip)**.

## Execução local

Como o projeto é composto por uma página HTML independente, basta abrir o arquivo:

```bash
open index.html
```

No Windows, você pode clicar duas vezes em `index.html`. Para servir o projeto em um servidor local:

```bash
python3 -m http.server 8000
```

Depois, acesse:

```text
http://localhost:8000
```

## GitHub Pages

O projeto pode ser publicado diretamente pelo GitHub Pages:

1. Acesse **Settings > Pages** no repositório.
2. Em **Build and deployment**, escolha **Deploy from a branch**.
3. Selecione a branch `main` e a pasta `/ (root)`.
4. Clique em **Save**.

## Tecnologias

- HTML5
- CSS3
- JavaScript
- Canvas API
- File API
- `createImageBitmap`
- [JSZip](https://stuk.github.io/jszip/) via CDN

## Privacidade

Todo o processamento é realizado no dispositivo do usuário. Nenhuma imagem é enviada ou armazenada em servidor pelo aplicativo.

## Estrutura

```text
imagemcut-studio/
└── index.html
```

## Navegadores

É recomendado utilizar uma versão atualizada do Chrome, Edge, Firefox ou Safari. Os formatos disponíveis para exportação dependem do suporte de conversão da API Canvas no navegador.

## Licença

Nenhuma licença foi definida neste repositório até o momento.
