<h1>ProjetoAPI</h1>

<p><strong>Desenvolvido por:</strong> Izabela e Maria Luiza</p>

<h2>Descrição do Projeto</h2>
<p>Essa API foi desenvolvida como parte de um exercício de aprendizado, com o objetivo de praticar o uso de rotas, métodos HTTP e manipulação de dados em uma aplicação web. Ela permite que usuários realizem operações básicas de CRUD (Criar, Ler, Atualizar e Deletar) de maneira simples e funcional.</p>

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

<h2>Exemplo de Requisição POST</h2>
<p>Para adicionar um novo item, envie um JSON para a rota <code>/api/dados</code> com o seguinte conteúdo:</p>
<pre>
{
  "nome": "Exemplo",
  "valor": 100
}
</pre>

<h2>Métodos HTTP usados</h2>
<ul>
  <li><strong>GET</strong> - Usado para buscar/visualizar dados</li>
  <li><strong>POST</strong> - Usado para criar novos registros</li>
  <li><strong>PUT</strong> - Usado para atualizar informações já existentes</li>
  <li><strong>DELETE</strong> - Usado para apagar registros</li>
</ul>

<h2>Ferramentas Recomendadas para Testar</h2>
<ul>
  <li>Postman</li>
  <li>Insomnia</li>
  <li>Navegador com extensões de requisição REST</li>
</ul>

<h2>Tecnologias Utilizadas</h2>
<ul>
  <li>Python</li>
  <li>Flask (framework web para criar a API)</li>
  <li>JSON (formato dos dados trafegados na API)</li>
</ul>

<h2>Possíveis Melhorias Futuras</h2>
<ul>
  <li>Adicionar conexão com banco de dados (como SQLite ou MySQL)</li>
  <li>Incluir autenticação de usuários</li>
  <li>Adicionar tratamento de erros e validações</li>
  <li>Documentar os endpoints com Swagger ou outra ferramenta</li>
</ul>

