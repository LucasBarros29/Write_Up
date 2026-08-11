# Cookie Admin

> Categoria: Web Exploitation

## Introdução

Este desafio aborda conceitos básicos de exploração web através da manipulação de cookies armazenados no navegador. O objetivo é identificar como a aplicação controla privilégios de usuário e obter acesso administrativo para encontrar a flag.

## Análise Inicial

Ao acessar o site, a seguinte mensagem era exibida:

> Cookie Monster 🍪
>
> NOM NOM... Você não é admin!

![Página Inicial](images/pagina-inicial.png)

As pistas fornecidas pelo desafio indicavam que a solução estava relacionada aos cookies da aplicação. Com isso, a principal hipótese foi que o status de administrador era controlado por um valor armazenado no navegador.

## Resolução

Utilizando as ferramentas de desenvolvedor do navegador (F12), acessei a seção de armazenamento de cookies para analisar os dados salvos pela aplicação.

Durante a inspeção foi encontrado um cookie responsável por definir se o usuário possuía privilégios administrativos.

![Cookie Original](images/cookie-original.png)

O valor indicava que o usuário não era administrador. Após modificar esse valor para representar um usuário administrador e atualizar a página, a aplicação passou a reconhecer a alteração.

![Cookie Alterado](images/cookie-alterado.png)

Depois da modificação, a página exibiu a seguinte mensagem:

> Cookie Monster 🍪
>
> NOM NOM NOM! DELÍCIA! Aqui está sua flag: FLAG{C00K1E_M0NST3R_MUNCH}

![Flag Obtida](images/flag.png)

## Flag

```text
FLAG{C00K1E_M0NST3R_MUNCH}
