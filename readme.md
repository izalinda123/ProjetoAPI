<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ProjetoAPI - Documentação</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            color: #333;
        }
        header {
            text-align: center;
            margin-bottom: 30px;
            padding-bottom: 20px;
            border-bottom: 1px solid #eee;
        }
        h1 {
            color: #0366d6;
        }
        h2 {
            color: #24292e;
            margin-top: 25px;
        }
        code {
            background-color: #f6f8fa;
            padding: 2px 4px;
            border-radius: 3px;
            font-family: monospace;
        }
        pre {
            background-color: #f6f8fa;
            padding: 10px;
            border-radius: 3px;
            overflow: auto;
        }
        .endpoint {
            background-color: #f0f7ff;
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>ProjetoAPI</h1>
        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/af76dd71-7e02-42d7-971e-805311e2a9c5.png" alt="Diagrama de arquitetura da API mostrando clientes se conectando a um servidor central" />
        <p>API RESTful para gerenciamento de recursos</p>
    </header>
    <section>
        <h2>Descrição</h2>
        <p>A ProjetoAPI é uma aplicação RESTful desenvolvida para facilitar o gerenciamento de dados através de endpoints seguros e padronizados. Nossa API fornece:</p>
        <ul>
            <li>Operações CRUD completas</li>
            <li>Autenticação via JWT</li>
            <li>Documentação Swagger integrada</li>
            <li>Rate limiting para segurança</li>
        </ul>
    </section>
    <section>
        <h2>Como Usar</h2>
        <div class="endpoint">
            <h3>GET /api/items</h3>
            <p>Lista todos os itens disponíveis</p>
            <pre><code>curl -X GET "https://api.exemplo.com/items"</code></pre>
        </div>
        <div class="endpoint">
            <h3>POST /api/items</h3>
            <p>Cria um novo item</p>
            <pre><code>curl -X POST "https://api.exemplo.com/items" \
-H "Content-Type: application/json" \
-H "Authorization: Bearer SEU_TOKEN_JWT" \
-d '{"nome": "Novo Item", "descricao": "Descrição do item"}'</code></pre>
        </div>
    </section>
    <section>
        <h2>Autenticação</h2>
        <p>Todas as requisições (exceto login) devem incluir o token JWT no header:</p>
        <pre><code>Authorization: Bearer SEU_TOKEN_JWT</code></pre>
    </section>
    <section>
        <h2>Variáveis de Ambiente</h2>
        <pre><code>API_PORT=3000
DB_URL=mongodb://localhost:27017/projetoapi
JWT_SECRET=secreto_aleatorio</code></pre>
    </section>
    <footer>
        <p>© 2023 ProjetoAPI. Todos os direitos reservados.</p>
    </footer>
</body>
</html>
