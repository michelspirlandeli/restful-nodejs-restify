## RESTful com Node.js, Restify e MySQL

### Pré-requisitos

- **Node.js** versão 8 ou superior;
- **Nodemon** - `npm i -g nodemon`.

### Instalação e Execução

1. Faça o clone do repositório e no terminal navegue até a pasta;
2. Instale as dependências do projeto com `npm install`;
3. Faça uma cópia do **.env.example** com o nome **.env** e adicione as informações de conexão com seu banco de dados MySQL (produção e teste). Não se esqueça de criar as tabelas:
```create table categories (id INT(11) unsigned not null auto_increment, name VARCHAR(255), primary key(id));CREATE TABLE `users` (
  `id` int(11) unsigned NOT NULL AUTO_INCREMENT,
  `email` varchar(255) NOT NULL DEFAULT '',
  `password` varchar(40) NOT NULL DEFAULT '',
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=utf8;```
4. Rode o servidor de desenvolvimento com `npm run dev`;
5. Rode os testes com `npm test`. Para observar os arquivos durante o desenvolvimento utilize `npm test -- --watch`;
6. O *endpoint* do serviço estará disponível em http://localhost:3456 .

### Sugestão

Utilize o Postman para testar suas chamadas. [https://www.getpostman.com/](https://www.getpostman.com/).

## Author
Michel Spirlandeli

## Github
https://github.com/michelspirlandeli