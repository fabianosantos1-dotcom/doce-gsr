#Este é um guia simples para configurar, rodar e publicar sua documentação.

Primeiro, instale o ambiente necessário executando o comando:

curl -LsSf https://astral.sh/uv/install.sh | sh

Depois, inicialize o projeto:

uv init

Em seguida, adicione as dependências do MkDocs e do tema Material:

uv add mkdocs mkdocs-material

Agora, crie a estrutura inicial da documentação:

uv run mkdocs new .

Com tudo configurado, você já pode rodar o projeto localmente:

uv run mkdocs serve

Abra o navegador e acesse http://127.0.0.1:8000 para visualizar.

Se precisar ajustar configurações, edite o arquivo mkdocs.yml.

Quando estiver pronto para publicar, faça o deploy:

uv run mkdocs gh-deploy

Por fim, versione e envie as alterações para o repositório:

git add .
git commit -m "MENSAGEM"
git push