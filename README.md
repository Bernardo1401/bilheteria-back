Como rodar o Back-End corretamente?

Clone este repositório no VSCode e instale as bibliotecas necessários com os seguintes códigos:
npm install express cors dotenv uuid

npm install nodemon --save-dev

Coloque o servidor para rodar com o seguinte comando: npm run dev
Abra o Postman, crie uma pasta com as seguintes 'requests':
image

Realizar as rotas: 4.1. Buscar todos os ingressos Dentro da rota GET adicione a seguinte URL: http://localhost:3000/api/ingressos Após clicar em 'Send', todos os ingressos devem aparecer.
4.2. Buscar um ingresso pelo ID Dentro da rota GET adicione a seguinte URL: http://localhost:3000/api/ingressos/id (colocar id) Após clicar em 'Send', deve aparecer o ingresso do ID inserido.

4.3. Criar um ingresso Dentro da rota POST adicione a seguinte URL: http://localhost:3000/api/ingressos E no body adicione as informações de "evento", "local", "data_evento", "categoria", "preco", "quantidade_disponivel". Ficando neste modelo:

![image](https://github.com/user-attachments/assets/f3cd7bc8-1885-4c20-93e9-a12ae861f075)

Após clicar em 'Send', o ingresso será adicionado.

4.4. Atualizar um ingresso Dentro da rota PUT adicione a seguinte URL: http://localhost:3000/api/ingressos/id (colocar id) E no body adicione as informações que você deseja atualizar ("evento", "local", "data_evento", "categoria", "preco", "quantidade_disponivel"). *As informações que não desejar alterar também devem ser inseridas. Após clicar em 'Send', o ingresso será atualizado:

![image](https://github.com/user-attachments/assets/7028f10b-cabe-4bec-ac8a-1e23820d1a0f)

4.5. Deletar um ingresso Dentro da rota DELETE adicione a seguinte URL: http://localhost:3000/api/ingressos/id (colocar id) Após clicar em 'Send', o ingresso será deletado, sendo possível confirmar com a mensagem de confirmação:

![image](https://github.com/user-attachments/assets/ee45b0a8-ecbe-4389-8f3a-db054e484fce)

4.6. Comprar um ingresso Dentro da rota POST adicione a seguinte URL: http://localhost:3000/api/venda No body, adicione o id do ingresso que deseja comprar e a quantidade de ingressos, como a imagem a seguir:

![image](https://github.com/user-attachments/assets/704f4e2d-a4d3-45ce-a67b-1812b133f556)

Após clicar em 'Send', a seguinte mensagem de confirmação deve aparecer: 

![image](https://github.com/user-attachments/assets/12a37a87-1e20-4e42-87cc-2ab5b8815844)
