# ITBR Australia — Website

Static recreation of the **ITBR Australia** site (Comunidade Brasileira de TI na Austrália),
rebuilt as clean, dependency-free HTML/CSS for hosting on **GitHub Pages**.

## Structure

```
itbr-new/
├── index.html          # Home
├── comunidades.html    # Comunidades
├── eventos.html        # Eventos
├── noticias.html       # Notícias
├── faq.html            # Perguntas frequentes
├── galeria.html        # Galeria de vídeos
├── links.html          # Links úteis
├── assets/
│   ├── css/style.css
│   ├── js/main.js
│   └── img/            # logo, fotos e imagens
└── .nojekyll           # impede o processamento Jekyll no GitHub Pages
```

## Rodar localmente

A partir da raiz do projeto, execute:

```powershell
./start.ps1
```

O script sobe um servidor estático e abre `http://localhost:8080` no navegador.

## Publicar no GitHub Pages

1. Faça commit do conteúdo desta pasta no repositório.
2. Em **Settings → Pages**, selecione a branch e a pasta `/itbr-new` (ou mova o conteúdo para a raiz / `docs`).
3. O site ficará disponível em `https://<usuario>.github.io/<repo>/`.

Como todos os caminhos são relativos, o site funciona em qualquer subdiretório.
