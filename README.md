Automação de Testes — SauceDemo (DESAFIO MUTANT)

Este projeto contém a automação de testes do site https://www.saucedemo.com/, utilizando Cypress.

O objetivo foi validar alguns fluxos principais da aplicação.


· Os seguintes cenários foram cobertos:

Login com sucesso
Login com credenciais inválidas
Adição de produto ao carrinho
Logout do sistema


· Tecnologias utilizadas:
JavaScript
Cypress
Node.js



· Estrutura do Projeto:

desafio_mutant
cypress/
├── e2e/
│   ├── login.cy.js
│   ├── login-failed.cy.js
│   ├── cart.cy.js
│   └── logout.cy.js
│
├── fixtures/
│   ├──example.json
├── support/
│   ├── commands.js
│   └── e2e.js
│
cypress.config.js
README.md




· Legenda da Estrutura do Projeto:

cypress/e2e/ → onde ficam os testes
fixtures/ → dados mockados (se necessário)
support/ → comandos customizados e configurações globais
cypress.config.js → configuração do Cypress


· Como instalar o projeto >

git clone <LINK_DO_REPOSITORIO> 
cd <NOME_DO_PROJETO>

· Instale as dependências:

npm install


· Como executar os testes

Modo interativo (interface do Cypress)
npx cypress open

Modo headless (terminal)
npx cypress run


· Evidências de execução:

O Cypress gera automaticamente evidências durante a execução:

Screenshots (em caso de falha)
Vídeos da execução

Esses arquivos ficam na pasta:

cypress/screenshots/
cypress/videos/


· Observações:
Os testes foram escritos de forma simples e direta, priorizando legibilidade
Os cenários simulam o fluxo real do usuário dentro da aplicação
A estrutura segue o padrão recomendado pelo Cypress