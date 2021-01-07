## Como criar um app React consumindo um back-end Node com Express


# Criando a base do projeto
O primeiro passo é criar o seu projeto React utilizando o pacote create-react-app (se você ainda não o conhece, clique aqui). Para isso, basta digitar o seguinte comando no terminal:
create-react-app node-react
A ferramenta do Facebook vai criar todo o código base para o projeto em React funcionar. Isso pode levar alguns minutos. Feito isso, entre na raiz do projeto, crie uma pasta chamada /client e mova todo o código gerado para dentro dela.

# O back-end com Express
Na raiz do projeto, junto a pasta /client que desenvolvemos no passo anterior, crie um novo arquivo chamado package.json (o ponto de partida de qualquer projeto NodeJS)

Aqui usaremos o pacote concurrently para rodar a aplicação React e o servidor ao mesmo tempo. Agora, crie um arquivo chamado server.js


Este código é uma simples API REST utilizando o Express. Em resumo, ele cria um endpoint em /api/mensagem e retorna uma simples mensagem “Hello from Express”. Iremos consumir esta API lá no front-end que já deixamos preparado.
Consumindo a API
Agora que já cuidamos da API, vamos retornar ao diretório /client. No arquivo package.json gerado pelo create-react-app,
