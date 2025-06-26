<h1>ProjetoAPI</h1>

<p>Essa API foi desenvolvida com o objetivo de treinar a criação de aplicações web que usam rotas e manipulam dados. Ela permite que o usuário visualize, cadastre, edite e apague informações por meio de requisições HTTP.</p>

<h2>O que a API faz</h2>
<ul>
  <li>Mostrar todos os dados cadastrados</li>
  <li>Adicionar novos dados</li>
  <li>Editar dados existentes</li>
  <li>Excluir dados da lista</li>
</ul>

<h2>Tecnologias utilizadas</h2>
<ul>
  <li>Python</li>
  <li>Flask (framework web)</li>
  <li>JSON (formato dos dados enviados e recebidos)</li>
</ul>

<h2>Como usar</h2>
<p>Você pode testar a API com ferramentas como Postman ou Insomnia, ou criar um front-end que se conecte às rotas.</p>

<pre>
GET     /api/dados        → Retorna todos os dados
POST    /api/dados        → Cria um novo dado
PUT     /api/dados/:id    → Atualiza o dado com o ID informado
DELETE  /api/dados/:id    → Remove o dado com o ID informado
</pre>

<h2>Exemplo de requisição POST</h2>
<p>Para adicionar um novo item, envie o seguinte JSON para a rota /api/dados:</p>

<pre>
{
  "nome": "Exemplo",
  "valor": 100
}
</pre>

<h2>Observações finais</h2>
<p>Esse projeto é básico, feito para fins de aprendizado. Pode ser expandido com autenticação, banco de dados, tratamento de erros e outras melhorias.</p>

<p>Desenvolvido por: IZABELA E MARIA LUIZA</p>
