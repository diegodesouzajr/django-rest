# django-rest
API com aplicação JWT e rest

Desenvolvimento de uma aplicação em Django em backend.

Adicionado método para cadastro de ususário. Realiza o login do usuário via token JWT.

Instalar as bibliotecas através do requirements.txt

Testes: python manage.py runserver

Criação do token com um usuário criado no sistema, executar no terminal o comando abaixo e o sistema irá te retornar o token para acesso ao sistema. $ curl -X POST -d "username=username&password=password" http://localhost:8000/login/

Para acessar as APIs protegidas, você deve incluir o Authorization: JWT cabeçalho. $ curl -H "Authorization: JWT " http://localhost:8000/protected-url/

Atualizar Token $ curl -X POST -H "Content-Type: application/json" -d '{"token":"<EXISTING_TOKEN>"}' http://localhost:8000/refresh-token/

Para testar a API: http://127.0.0.1:8000/usuario/

Todas as urls podem ser testadas via Postman, passando os parâmetros na autenticação e no formulário.
