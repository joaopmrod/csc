# Coimbra Ski Club - Landing Page

Esta é a landing page estática para o **Coimbra Ski Club**, pronta a ser publicada no GitHub Pages.

## Tecnologias Utilizadas
- **HTML5**
- **Tailwind CSS** (via CDN para facilitar a publicação estática sem necessidade de build steps)
- **Font Awesome** (Ícones)
- **Google Fonts** (Montserrat)

## Como publicar no GitHub Pages

1. Faz commit e push deste código para o teu repositório no GitHub:
   ```bash
   git add .
   git commit -m "Initial commit: Landing page Coimbra Ski Club"
   git branch -M main
   git push -u origin main
   ```

2. No GitHub, vai à página do teu repositório.
3. Clica em **Settings** (Definições) no menu superior.
4. Na barra lateral esquerda, clica em **Pages**.
5. Na secção "Build and deployment", em **Source**, seleciona **Deploy from a branch**.
6. Em **Branch**, seleciona `main` (ou `master`) e a pasta `/ (root)`.
7. Clica em **Save**.
8. Aguarda alguns minutos e o teu site estará disponível no link fornecido pelo GitHub (normalmente `https://[teu-username].github.io/[nome-do-repo]`).

## Notas sobre o Formulário de Contacto

Como o GitHub Pages apenas aloja ficheiros estáticos (HTML/CSS/JS), não é possível processar formulários diretamente com PHP ou Node.js. 

Para que o formulário funcione e envie emails reais:
1. Cria uma conta gratuita no [Formspree](https://formspree.io/).
2. Cria um novo formulário no Formspree.
3. Copia o URL fornecido (ex: `https://formspree.io/f/xabcdefg`).
4. Abre o ficheiro `index.html`.
5. Procura pela tag `<form action="https://formspree.io/f/YOUR_FORM_ID_HERE"...`.
6. Substitui `YOUR_FORM_ID_HERE` pelo ID do teu formulário Formspree.
7. Remove o código JavaScript no final do ficheiro que impede o envio real do formulário (procura por `e.preventDefault();` na secção Form Submission Simulation).