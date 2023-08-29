# DESAFIO-API-PHP

Esse desafio tem como objetivo criar uma API em PHP e consumi-la com JavaScript. Para isso, você deverá usar o método FETCH nativo da linguagem JavaScript, ou, se preferir, pode optar por utilizar alguma biblioteca para fazer requisições à API, fica a seu critério.

## Primeiros passos

1. Você deverá dar um fork no repositório, fazendo isso ele será copiado para o seu GitHub.
2. Clone o repositório para sua maquina, crie uma branch com seu nome e codifique na branch criada.
```
$ git clone link-do-seu-repositorio
```
3. Após o clone você deverá criar uma branch com seu nome e codificar nela.

## Como testar a API?

Para testar a API, você pode utilizar o software Insomnia ou Postman, de acordo com sua preferência. Dentro do software, informe a URL e selecione o tipo de requisição que deseja fazer para o seu ENDPOINT (GET, POST, PUT ou DELETE). Se for bem-sucedido, você deve retornar uma resposta no formato JSON.

## Back-end

Salvar no banco os seguintes campos. 
```php
ID NAME EMAIL CPF PASSWORD CREATED_AT UPDATED_AT
```
Ao criar um registro, o campo CREATED_AT deve ser preenchido com a data em que o registro foi criado. O campo UPDATED_AT deve ser preenchido somente quando o registro for atualizado, com a data exata em que a atualização ocorreu.

### O que validar?

- O campo de e-mail deve ser validado para garantir que seja um endereço de e-mail válido e que não exista um e-mail igual já cadastrado no banco de dados.
- O campo CPF deve ser validado para garantir que seja um CPF válido e que não exista um CPF igual já cadastrado no banco de dados.
- O campo de senha (password) deve ser armazenado no banco de dados utilizando uma técnica de segurança chamada "hashing" (HASH) para garantir que, em caso de invasão, as senhas não estejam vulneráveis. Você pode utilizar o método nativo do PHP ```hash()``` para isso.
- Os campos created_at e updated_at devem ser armazenados seguindo o formato de datas do banco de dados, por exemplo, "**1999-10-10**".


## Recursos

Aqui estão alguns recursos úteis que podem ajudá-lo a completar este desafio:

- [Documentação do PHP](https://www.php.net/docs.php)
- [Documentação do JavaScript](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
- [MDN Web Docs - Fetch API](https://developer.mozilla.org/pt-BR/docs/Web/API/Fetch_API)

