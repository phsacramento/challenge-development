## Overview

O Github é uma rede social de programadores que possui uma funcionalidade interessante que permite curtir o repositório alheio. Trata-se de um botão escrito Star encontrado na página de cada repositório.  
Rick é um usuário ativo do Github que está sempre buscando novos projetos curtindo os que acha interessantes. Ele gostaria de poder adicionar um label ou tag para marcar o repositório de modo que ele possa filtrar. Por exemplo, ele encontrou um repositório chamado `react` e gostaria de adicionar as tags `javascript` e `frontend`.  
Como o Github não possui essa funcionalidade, Rick precisa de um sistema que consiga ajudá-lo com isso.

## O que vai ser avaliado?

Queremos avaliar sua capacidade em entregar um produto completo e com documentação mínima suficiente para outros desenvolvedores conseguirem contribuir com o projeto. É essencial que o `README.md` contenha as intruções para configurar e rodar o projeto, bastanto apenas um ctrl+c/ctrl+v no terminal do Linux e do OSX para conseguir rodar a aplicação.     
Outros pontos que vamos considerar na avaliação:

- Código bem escrito, limpo e coeso utilizando os princípios [SOLID](https://www.google.com.br/search?q=principios+solid&oq=principios+solid)
- Implementação da solução
- Design da API RESTful, utilizando corretamente os verbos `HTTP` e os devidos `STATUS CODE`
- Testes automatizados do front-end e da API
- Cobertura de testes
- Linter/Análise estática do código de acordo com a linguagem
- Documentação da API utilizando API Blueprint, **NÃO** pdf, txt ou qualquer outro formato
- Conhecimento em Javascript, HTML5 e CSS3
- Capacidade de implementar as telas **EXATAMENTE** como está no wireframe fornecido, considerando a posição dos elementos na tela
- README.md bem escrito, curto e com os comandos necessários para rodar a aplicação

## Instruções

1. Crie um arquivo `README.md` descrevendo como configurar o projeto, contendo os comandos que devem ser executados para rodar o software e os testes;
2. Crie um ZIP do projeto sem as dependências instaladas;
3. Disponibilize o arquivo para download e nos envie a URL por email.

## Tecnologias

Na brainn não trabalhamos com uma linguagem ou um framework apenas. Somos poliglotas e incentivamos o uso de novas tecnologias desde que o time concorde em conjunto e esteja preparado para assumir os riscos da implementação. Nesse momento, nossas opções são específicas do nosso time. Escolha entre as opções abaixo para o desafio:

* Javascript
* Python
* Ruby
* Golang
* React
* Vue

## Desafio

O desafio consiste em desenvolver uma aplicação web que obtém todos os repositórios que um determinado usuário "curtiu" e salvar em um banco de dados local para permitir associar tags (labels ou hashtags) à cada repositório. Atualmente o Github não possui esse recurso e fica difícil classificar projetos open source interessantes.
O projeto deve funcionar com o front-end utilizando consultas AJAX para transferir informações ao back-end.

Há 3 user stories para entendimento sobre o que é necessário fazer:

### 1. Obter repositórios remotos e cadastrar no banco de dados local

> Como usuário, eu quero fornecer meu username e salvar no banco de dados local todos os repositórios que eu curti para depois conseguir adicionar minhas tags.

#### Wireframe

![Tela 1](wireframes/01.png?raw=true "Insira o username")
![Tela 2](wireframes/02.png?raw=true "Loading...")

#### Cenário

O usuário informa o username na tela para que o sistema obtenha os repositórios do Github.

#### Critérios de Aceitação

* Deve obter os repositórios com star utilizando a API Rest v3 do Github. Utilizar a API v4 com GraphQL é um plus.
* As informações que devem ser salvas no banco de dados são: ID do repositório, nome do repositório, descrição, URL HTTP e linguagem.

### 2. Adicionar tags para os repositórios

> Como usuário, eu quero poder adicionar tags (labels) para cada repositório para eu poder efetuar uma busca por tag.

#### Wireframe

![Tela 3](wireframes/03.png?raw=true "Lista de todos os repositórios")
![Tela 4](wireframes/04.png?raw=true "Adicionando tag")

#### Cenário

O usuário acessa o sistema pelo browser, visualiza a lista de repositórios cadastrados no banco de dados, seleciona um deles e consegue digitar tags separadas por vírgula para salvar em seguida.

#### Critérios de Aceitação

* Um repositório não pode ter tags duplicadas.

### 3. Buscar repositórios por tag

> Como usuário, quero poder fornecer uma tag e obter os repositórios que possuem essa tag para visualizar na tela o resultado da minha busca.

#### Wireframe

![Tela 5](wireframes/05.png?raw=true "Busca por tag")

#### Cenário

O usuário acessa o sistema, digita uma tag e aperta a tecla <Enter>. O sistema exibe todos os repositórios que tenham a tag definida.

#### Critérios de Aceitação

* A busca precisa consultar o back-end


## Considerações Finais

Entendemos as dificuldades do dia-a-dia para quem trabalha em ter que dedicar um tempo para resolver esse tipo de desafio. Por isso pedimos para que mesmo que você não consiga completar o desafio, nos envie assim mesmo. Não queremos julgar nossos candidatos, queremos apenas entender melhor a maneira como cada um pensa e age diante de um problema comum.  

Qualquer dúvida pode entrar em contato conosco.  

Boa sorte!!!
