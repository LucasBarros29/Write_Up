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

O valor do cookie indicava que o usuário não possuía privilégios administrativos. Após alterar esse valor para representar um usuário administrador e atualizar a página, a aplicação passou a reconhecer a alteração.

A página então exibiu a seguinte mensagem:

> Cookie Monster 🍪
>
> NOM NOM NOM! DELÍCIA! Aqui está sua flag: FLAG{C00K1E_M0NST3R_MUNCH}

## Flag

```text
FLAG{C00K1E_M0NST3R_MUNCH}
```

## Conclusão

Este desafio demonstra um conceito básico de segurança web: informações armazenadas no lado do cliente não devem ser consideradas confiáveis. Ao manipular um cookie responsável pelo controle de permissões, foi possível obter privilégios administrativos e acessar a flag. Além disso, o desafio reforça a importância de utilizar as ferramentas de desenvolvedor do navegador para analisar o funcionamento de aplicações web.
