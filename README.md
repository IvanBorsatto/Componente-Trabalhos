# Variáveis do CSS

- São valores que podemos definir e usar no decorrer do projeto.
    
    ```bash
    Exemplo:
    :root {
      --ff-heading:'Epilogue', sans-serif;
      --ff-texting: 'Opens sans', sans-serif;
    
      --hue:250;
      --bg-primary: hsl(var(--hue), 22%, 20%);
      --fc-primary: hsl(var(--hue), 0%, 100%);
      --fc-secondary: hsl(var(--hue), 50%,80%);
      --fc-secondary-dark: hsl(var(--hue), 100%, 11%, 1);
    
      font-size: 62.5%;
      --fs-body: 1.6rem;
      --fs-heading: 4rem; 
    }
    ```
    

- **object-fit: cover;** = Para encaixar um conteúdo dentro de uma caixa;
- **width: fit-content;** = Vai encaixar o elemento no conteúdo;
- Transition e Transformação de elementos
    - **transform: ;** = Para indicar qual movimento este conteúdo irá fazer ao passar o mouse em cima do conteúdo (tag seguida de :hover);
    - **transition: ;** = Define o tempo que do movimento completo do conteúdo ( se utiliza esta opção dentro da tag sem o :hover)
    
    ```bash
    Exemplo:
    .card img {
      width: 41.6rem;
      object-fit: cover;
    
      border-radius: 6px;
    
      transition: transform 200ms;
    }
    
    .card img:hover {
      transform: scale(1.1);
    }
    ```
    

- ANIMAÇÕES CSS
    
    ```bash
    @keyframes "declaro nome que eu quiser" {
      0% {
    
      }
    
      100% {
    
      }
    }
    
    Exemplo:
    header {
      animation-name: topdown;
      animation-duration: 700ms;
      animation-fill-mode: forwards;
      animation-duration: reverse;
      animation-delay: 200ms;
      animation-timing-function: ease;
      animation-iteration-count: infinite;
      animation-play-state: paused;
    }
    
    header:hover {
      animation-play-state: running;
    }
    
    @keyframes topdown {
      0% {
        opacity: 0;
        transform: translateY(-15px);
      }
    
      50% {
        opacity: 1;
      }
    
      100% {
        opacity: 0;
        transform: translateY(0);
      }
    }
    ```
    

- **main div:nth-child(1)** = Informa que é para pegar a primeira div dentro o main e inserir as configurações ela;
- **clamp** = Flexibilidade nos tamanhos dos textos no CSS