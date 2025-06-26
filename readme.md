<h1>ProjetoAPI</h1>

<p><strong>Desenvolvido por:</strong> Izabela e Maria Luiza</p>

<h2>Descrição do Projeto</h2>
<p>Essa API foi desenvolvida como parte de um exercício de aprendizado, com o objetivo de praticar o uso de rotas, métodos HTTP e manipulação de dados em uma aplicação web. Ela permite que usuários realizem operações básicas de CRUD (Criar, Ler, Atualizar e Deletar).</p>

<h2>Funcionalidades da API</h2>
<ul>
  <li>Visualizar todos os dados cadastrados</li>
  <li>Adicionar um novo dado</li>
  <li>Editar dados existentes com base no ID</li>
  <li>Excluir dados do sistema</li>
</ul>

<h2>Rotas Disponíveis</h2>
<pre>
GET     /api/dados        → Retorna todos os dados cadastrados
POST    /api/dados        → Cadastra um novo dado
PUT     /api/dados/:id    → Atualiza um dado existente usando o ID
DELETE  /api/dados/:id    → Remove um dado com base no ID
</pre>

<h2>Exemplos de Requisições</h2>

<h3>GET /api/dados</h3>
<p>Usado para buscar todos os dados cadastrados.</p>
<pre>
Resposta:
[
  {
    "id": 1,
    "nome": "Produto A",
    "valor": 50
  },
  {
    "id": 2,
    "nome": "Produto B",
    "valor": 75
  }
]
</pre>

<h3>POST /api/dados</h3>
<p>Usado para adicionar um novo dado.</p>
<pre>
Corpo da requisição:
{
  "nome": "Produto C",
  "valor": 100
}

Resposta:
{
  "mensagem": "Dado criado com sucesso",
  "id": 3
}
</pre>

<h3>PUT /api/dados/1</h3>
<p>Usado para atualizar um dado com ID 1.</p>
<pre>
Corpo da requisição:
{
  "nome": "Produto A - Atualizado",
  "valor": 60
}

Resposta:
{
  "mensagem": "Dado atualizado com sucesso"
}
</pre>

<h3>DELETE /api/dados/2</h3>
<p>Usado para deletar o dado com ID 2.</p>
<pre>
Resposta:
{
  "mensagem": "Dado removido com sucesso"
}
</pre>

<h2>Explicação dos Métodos HTTP</h2>
<ul>
  <li><strong>GET:</strong> Buscar ou visualizar dados existentes</li>
  <li><strong>POST:</strong> Criar um novo dado</li>
  <li><strong>PUT:</strong> Atualizar informações de um dado já existente</li>
  <li><strong>DELETE:</strong> Apagar um dado</li>
</ul>

<h2>Tecnologias Utilizadas</h2>
<ul>
  <li>Python</li>
  <li>Flask (framework web para criação da API)</li>
  <li>JSON (formato usado para enviar e receber os dados)</li>
</ul>

<h2>Ferramentas Recomendadas para Testar</h2>
<ul>
  <li>Postman</li>
  <li>Insomnia</li>
  <li>Extensões REST Client para o VS Code</li>
</ul>

<h2>Como rodar o projeto localmente</h2>
<ol>
  <li>Tenha o Python instalado na sua máquina</li>
  <li>Instale o Flask com o comando: <code>pip install flask</code></li>
  <li>Crie um arquivo chamado <code>app.py</code> com o código da API</li>
  <li>No terminal, execute: <code>python app.py</code></li>
  <li>Acesse a API no navegador ou pelo Postman: <code>http://localhost:5000</code></li>
</ol>

<h2>Possíveis Melhorias Futuras</h2>
<ul>
  <li>Adicionar autenticação de usuários</li>
  <li>Salvar os dados em banco de dados (SQLite, MySQL ou MongoDB)</li>
  <li>Incluir tratamento de erros (ex: dado não encontrado)</li>
  <li>Documentar os endpoints com Swagger ou outra ferramenta</li>
</ul>

  <li>Documentar os endpoints com Swagger ou outra ferramenta</li>
</ul>

