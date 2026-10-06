# Cigano Motos — arquivos fonte

Landing page institucional em HTML, CSS e JavaScript puro, sem dependências ou etapa de compilação.
Exportação de 06/10/2026, com o logo enviado no cabeçalho e rodapé e os textos sem itálico.

## Estrutura

- `index.html`: estrutura, conteúdo e ícones SVG da página.
- `assets/css/styles.css`: cores, tipografia, layout responsivo e animações.
- `assets/js/main.js`: WhatsApp, janela de contato, ano e animações ao rolar.
- `assets/images/logo-cigano.png`: logo da oficina.
- `assets/images/hero.png`: imagem principal.
- `original/index.html`: cópia exata do HTML original da exportação.

## Abrir e executar

Extraia o ZIP e abra o `index.html` da pasta principal em um navegador.
Para editar no VS Code, abra a pasta `cigano-motos-fonte`.
Opcionalmente, use a extensão Live Server ou execute, nesta pasta:

```bash
python -m http.server 8000
```

Acesse http://localhost:8000. No Windows, se necessário, use `py -m http.server 8000`.

## Configurar WhatsApp

Em `assets/js/main.js`, preencha `WHATSAPP_NUMBER` com o número oficial, incluindo 55 e DDD, apenas dígitos.
Edite `message` para alterar a mensagem inicial. O número está vazio na versão exportada: enquanto não for configurado, os botões exibem a janela de contato pendente.

## Editar conteúdo e visual

Altere os textos em `index.html`, estilos em `assets/css/styles.css` e imagens em `assets/images/`.
As variáveis `--yellow`, `--black` e `--muted` controlam as cores principais.
Preserve os nomes das imagens ou atualize os caminhos em `index.html`.
A imagem do logo contém sua própria arte; a remoção do itálico aplica-se aos textos HTML.

## Hospedar

Envie o `index.html` principal e a pasta `assets` para uma hospedagem estática, preservando os caminhos.
A pasta `original` e este README não são necessários para publicar.
Não há servidor de aplicação, banco de dados, npm ou bibliotecas externas.

O pacote preserva o conteúdo e os recursos da versão exportada; apenas separa o CSS e JavaScript para facilitar manutenção. A exportação não altera o site publicado.
