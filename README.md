# Portfólio Pessoal Dinâmico

<div align="center">
  <img src="https://img.shields.io/badge/HTML-5-orange?style=for-the-badge&logo=html5" alt="HTML Badge" />
  <img src="https://img.shields.io/badge/CSS-3-blue?style=for-the-badge&logo=css3&logoColor=white" alt="CSS Badge" />
  <img src="https://img.shields.io/badge/JavaScript-ES6+-yellow?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript Badge" />
</div>

<p align="center">
  <a href="https://brunogodoy2911.github.io/portfolio_fundweb/"><strong>Acessar Demonstração »</strong></a>
</p>

## Visão Geral

Este é um projeto de site de portfólio pessoal de página única, projetado para ser moderno e responsivo. O diferencial deste portfólio é a sua capacidade de buscar e exibir informações de perfil diretamente da API do GitHub, como foto, biografia, número de seguidores e repositórios públicos.

O projeto também inclui um formulário de contato funcional com validação de campos.

## ✨ Recursos

- **Design Responsivo**: Totalmente adaptável para visualização em desktops e dispositivos móveis.
- **Conteúdo Dinâmico**: A seção "Sobre mim" é preenchida automaticamente com dados da API do GitHub.
- **Formulário de Contato**: Inclui um formulário com validação em JavaScript e utiliza o serviço [FormSubmit](https://formsubmit.co/) para o envio de e-mails.
- **Estilização Moderna**: Interface limpa com uso de variáveis CSS para um tema de cores consistente.

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura e semântica do conteúdo.
- **CSS3**: Estilização, layout e responsividade.
- **JavaScript (ES6+)**: Manipulação do DOM, validação de formulário e requisições à API do GitHub (`fetch`).

## 🚀 Executando Localmente

Para visualizar e testar o projeto em sua máquina local, siga os passos abaixo.

### Pré-requisitos

- Um editor de código de sua preferência (ex: [Visual Studio Code](https://code.visualstudio.com/)).
- A extensão **Live Server** para o VS Code (ou um servidor local similar).

### Passos

1.  Clone o repositório para a sua máquina:
    ```bash
    git clone [https://github.com/Brunogodoy2911/portfolio_fundweb.git](https://github.com/Brunogodoy2911/portfolio_fundweb.git)
    ```
2.  Abra a pasta do projeto no Visual Studio Code:
    ```bash
    cd portfolio_fundweb
    code .
    ```
3.  Com o arquivo `index.html` aberto, clique com o botão direito e selecione a opção **"Open with Live Server"**.

Isso abrirá o site no seu navegador padrão.

## ⚙️ Como Usar

Para adaptar este portfólio para seu próprio uso, você precisará alterar:

1.  **API do GitHub**: No arquivo `assets/js/script.js`, altere o nome de usuário na URL da API para o seu:
    ```javascript
    // Linha 6
    const dadosPerfil = await fetch(
      `https://api.github.com/users/SEU_USUARIO_AQUI`
    );
    ```

2.  **Formulário de Contato**: No arquivo `index.html`, substitua o endpoint na `action` do formulário pelo seu link do FormSubmit:
    ```html
    <form
      action="[https://formsubmit.co/SEU_EMAIL_AQUI](https://formsubmit.co/SEU_EMAIL_AQUI)"
      method="POST"
      id="formulario"
    >
    ```

3.  **Links das Redes Sociais**: Atualize os links para seu LinkedIn e GitHub no arquivo `index.html`.
