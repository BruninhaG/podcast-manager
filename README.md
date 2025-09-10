# Gerente de Podcast

> Uma aplicação inspirada no estilo da Netflix que centraliza e organiza episódios de podcasts em vídeo por categoria.

## 📝 Sobre o Projeto

O **Gerente de Podcast** é uma aplicação que busca facilitar o acesso e a organização de episódios de podcasts em formato de vídeo. Inspirado na experiência de navegação da Netflix, o projeto proporciona uma interface intuitiva e agradável, permitindo que os usuários explorem e encontrem seus conteúdos favoritos de forma eficiente.

## 🚀 Funcionalidades

* **Listagem por Categoria:** Navegue por sessões de episódios organizadas por categorias como `saúde`, `esporte`, `mentalidade` e `humor`.
* **Filtragem por Nome:** Encontre rapidamente episódios específicos buscando pelo nome do podcast.

## 💻 Tecnologias Utilizadas

* **[TypeScript](https://www.typescriptlang.org/)**: Linguagem de programação utilizada para o desenvolvimento, garantindo tipagem segura e código escalável.
* **[Node.js](https://nodejs.org/)**: Ambiente de execução JavaScript para o lado do servidor.
* **[Tsup](https://tsup.egoist.dev/)**: Ferramenta de empacotamento para projetos TypeScript, otimizando a construção do código.
* **[Tsx](https://github.com/esbuild-kit/tsx)**: Compilador TypeScript que facilita a execução e o desenvolvimento.
* `@types/node`: Pacote de definições de tipos para o Node.js.

## 💡 Instalação e Uso

Siga os passos abaixo para rodar a aplicação em sua máquina local.

### Pré-requisitos

O Node.js e o npm instalados.

### Passos

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
    cd seu-repositorio
    ```
2.  **Instale as dependências:**
    ```bash
    npm install
    ```
3.  **Inicie o servidor:**
    ```bash
    npm run start:dev
    ```
4.  Acesse os endpoints da API para interagir com a aplicação.

## ⚙️ Endpoints da API

* `GET /list`
    * **Descrição:** Retorna uma lista de episódios de podcasts, organizados por categorias.
    * **Exemplo de Resposta:**
        ```json
        [
          {
            "podcastName": "flow",
            "episode": "CBUM - Flow #319",
            "videoId": "pQSuQmUfS30",
            "cover": "[https://i.ytimg.com/vi/pQSuQmUfS30/maxresdefault.jpg](https://i.ytimg.com/vi/pQSuQmUfS30/maxresdefault.jpg)",
            "link": "[https://www.youtube.com/watch?v=pQSuQmUfS30](https://www.youtube.com/watch?v=pQSuQmUfS30)",
            "categories": ["saúde", "esporte", "bodybuilder"]
          },
          ...
        ]
        ```

* `GET /episode?podcastName={nome}`
    * **Descrição:** Retorna uma lista de episódios de podcast com base no nome do podcast fornecido.
    * **Exemplo de Requisição:**
        ```
        GET /episode?podcastName=flow
        ```

## 🤝 Como Contribuir

Contribuições são **muito bem-vindas**! Sinta-se à vontade para abrir [issues](link para a página de issues) ou enviar [pull requests](link para a página de pull requests) para ajudar a melhorar o projeto.


---
*Este README foi criado com base em templates e boas práticas para projetos open source.*
