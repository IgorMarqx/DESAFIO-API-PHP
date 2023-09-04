# Desafio API PHP e JavaScript

Esse desafio tem como objetivo criar uma API em PHP e consumi-la com JavaScript. Para isso, você deverá usar o método `FETCH` nativo da linguagem JavaScript, ou, se preferir, pode optar por utilizar alguma biblioteca para fazer requisições à API, fica a seu critério.

**Observação:**  `Antes de prosseguir para a construção da interface do FRONT e consumir a API, você deve testar completamente a API usando o Insomnia ou o Postman.`

## Configuração Inicial

1. Você deve dar um fork nesse repositório, fazendo isso ele será copiado para o seu GitHub.
2. Clone o repositório para sua maquina.
```php
$ git clone link-do-seu-repositorio
```
3. Após o clone você deverá criar uma branch com seu nome e codificar nela.
```php
$ git branch (para verificar em qual branch você estar)
```

## Testando a API

Para testar a API, você pode utilizar o software Insomnia ou Postman, de acordo com sua preferência. Dentro do software, informe a URL para seu endpoint e selecione o tipo de requisição que deseja fazer para o seu ENDPOINT (GET, POST, PUT ou DELETE). Se for bem-sucedido, você deve retornar uma resposta no formato JSON.

**Observação:** `Ao final do README, você encontrará alguns links úteis. Lá, você encontrará os links para instalar um desses softwares.`

### O que é um endpoint
- O endpoint da API representa um endereço ao qual o front-end se conecta para acessar uma funcionalidade específica. Em termos mais simples, o endpoint é a URL associada ao controller da API. Por exemplo, o controller é onde os dados são recebidos e inseridos no banco de dados.
- Você consegue acessar e testar esses endpoint pelos softwares citados acima.

## Desenvolvimento Back-End

Com base no que foi aprendido no desafio anterior objetivo principal desse desafio é criar um CRUD (CREATE, READ, UPDATE, DELETE), seguindo as regras a seguir:

Salvar no banco os seguintes campos. 
```php
$ id name email cpf password created_at updated_at
```
Ao criar um registro, o campo CREATED_AT deve ser preenchido com a data e hora em que o registro foi criado. O campo UPDATED_AT deve ser preenchido somente quando o registro for atualizado, com a data e hora exata em que a atualização ocorreu.

**Observação1:** `Os campos "created_at" e "updated_at" não devem ser enviados como parâmetros. O campo "created_at" deve ser incrementado automaticamente na criação e o campo "updated_at" na atualização.`

**Observação2:** `A conexão com o banco de dados deve ser estabelecida utilizando a biblioteca nativa do PHP conhecida como PDO (PHP Data Objects).`

### Validando os dados

- O campo de e-mail deve ser validado para garantir que seja um endereço de e-mail válido e que não exista um e-mail igual já cadastrado no banco de dados.
- O campo CPF deve ser validado para garantir que seja um CPF válido e que não exista um CPF igual já cadastrado no banco de dados.
- O campo de senha (password) deve ser armazenado no banco de dados utilizando uma técnica de segurança chamada "hashing" (HASH) para garantir que, em caso de invasão, as senhas não estejam vulneráveis. Você pode utilizar o método nativo do PHP `hash()` para isso.

## Desenvolvimento Front-End
**Observação:** `Antes de prosseguir para a construção da interface do FRONT e consumir a API, você deve testar completamente a API usando o Insomnia ou o Postman.`

- Desenvolva o front-end seguindo as melhores práticas de desenvolvimento.
- Utilize o método `fetch` nativo do JavaScript ou bibliotecas de sua escolha para fazer requisições à API.
- Crie uma interface de usuário que permita aos usuários realizar operações na API, como listar, criar, atualizar e excluir recursos.

## Desenvolvimento Back-End Avançado (OPCIONAL)
Neste tópico, apresento alguns desafios mais avançados que são inteiramente opcionais, mas consistem no seguinte:

- Aplicar programação orientada a objetos (POO) envolvendo a criação de classes e métodos para cada funcionalidade.
- Dividir as funcionalidades, atribuindo responsabilidades específicas a cada componente. Por exemplo, criar uma classe dedicada à inserção de dados no banco de dados, seguindo o padrão comumente denominado "repository pattern", e outra classe dedicada às validações, semelhante aos "form requests" no Laravel. Isso permite manter o controlador completamente limpo, concentrando-se apenas na geração da resposta necessária em formato JSON.

## Links úteis

Aqui estão alguns recursos úteis que podem ajudá-lo a completar este desafio:

- [Documentação do PHP](https://www.php.net/manual/pt_BR/index.php)
- [MDN Web Docs - Fetch API](https://developer.mozilla.org/pt-BR/docs/Web/API/Fetch_API)
- [Insomnia](https://insomnia.rest/download)
- [PostMan](https://www.postman.com/downloads/)
- [Detalhes sobre EndPoint API](https://mailchimp.com/pt-br/resources/what-is-an-api-endpoint/#:~:text=O%20endpoint%20de%20API%20é,de%20comunicação%20entre%20dois%20sistemas.)

## Desenvolvimento avançado links úteis
- [Repository Pattern](https://www.mitrais.com/news-updates/repository-pattern-implementation-in-php/)

<p align="center">
Boa sorte e divirta-se codificando! 💜
</p>
