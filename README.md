# Shelf

Site do Shelf: auditoria de estoque e quebra para o varejo alimentício.

Publicado com GitHub Pages a partir da branch `main`. O site inteiro está em `index.html` (logomarca, ilustração e ícones embutidos).

## Arquivos

| Arquivo | Função |
|---|---|
| `index.html` | O site completo. Funciona sozinho em qualquer hospedagem estática. |
| `og.png` | Imagem de compartilhamento (WhatsApp, LinkedIn, redes sociais), 1200 × 630 px. |
| `apple-touch-icon.png` | Ícone usado quando o site é adicionado à tela inicial do iPhone. |
| `favicon.svg` | Ícone da aba do navegador (também embutido no `index.html`). |
| `.nojekyll` | Faz o GitHub Pages publicar os arquivos como estão. |

## Formulários e contatos

Em `index.html`, procure por `CONFIG` e preencha:

- `endpoint`: endereço **https** que recebe os pedidos em JSON (Formspree, webhook de CRM ou backend do Shelf). Enquanto estiver vazio, o visitante recebe um resumo do pedido para enviar por e-mail ou WhatsApp.
- `email` e `whatsapp`: preenchem sozinhos a seção de contato, o rodapé, os botões "Copiar" e a tela de confirmação. Com eles definidos, a tela de confirmação também oferece "Enviar por e-mail" e "Enviar pelo WhatsApp" com o resumo pronto.

Os formulários têm um campo-armadilha contra robôs chamado `_gotcha` (compatível com o Formspree).

## Ao trocar de domínio

Atualize as três URLs com `franklingeronymo.github.io/shelf` no início do `index.html` (`canonical`, `og:url` e `og:image`).

## Pendências

Textos entre colchetes, como `[E-MAIL]`, `[PREÇO]` e `[CNPJ]`, aguardam definição do time.
