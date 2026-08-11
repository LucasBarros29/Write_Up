# Cookie Admin

> Categoria: Web Exploitation

## Introdução

Desafio simples de exploração web focado na manipulação de cookies armazenados pelo navegador.

## Análise Inicial

Ao acessar o site, a página exibia a mensagem:

> Cookie Monster 🍪
>
> NOM NOM... Você não é admin!

As dicas fornecidas indicavam que a solução estava relacionada aos cookies da aplicação.

## Resolução

Utilizando as ferramentas de desenvolvedor do navegador (F12), acessei a seção de armazenamento de cookies e identifiquei um cookie responsável por controlar o status de administrador.

O valor do cookie indicava que o usuário não possuía privilégios administrativos. Após alterar esse valor para representar um usuário administrador e atualizar a página, o comportamento da aplicação mudou e a flag foi exibida.

## Flag

> FLAG{C00K1E_M0NST3R_MUNCH}
