# 🍪 Cookie Admin

> 📂 Categoria: Web Exploitation

## 🎯 Introdução

Este desafio aborda conceitos básicos de exploração web por meio da manipulação de cookies armazenados pelo navegador. O objetivo é analisar o comportamento da aplicação e identificar como ela controla os privilégios de acesso dos usuários.

## 🔍 Análise Inicial

Ao acessar o site, nos deparamos com a seguinte mensagem:

> Cookie Monster 🍪
>
> NOM NOM... Você não é admin!

A página não apresentava muitas informações além dessa mensagem, o que indicava que a verificação de privilégios poderia estar ocorrendo por meio de algum dado armazenado localmente.

A tela inicial do desafio pode ser observada abaixo:

![Página Inicial](https://github.com/LucasBarros29/Write_Up/blob/main/Imagens/cookie01.png)

## 💡 Interpretação

O nome do desafio e a mensagem exibida sugerem que os cookies desempenham um papel importante na aplicação. Como cookies são frequentemente utilizados para armazenar informações de sessão e preferências do usuário, uma hipótese plausível era que o status de administrador estivesse sendo controlado por um valor armazenado no navegador.

## ⚙️ Resolução

Para verificar essa hipótese, foi utilizada a ferramenta de desenvolvedor do navegador (**F12**). Na seção de armazenamento de cookies, foi identificado um cookie responsável pelo controle de privilégios do usuário.

Ao analisar seu conteúdo, foi possível observar que o valor indicava que o usuário não possuía permissões administrativas. Após alterar esse valor para representar um usuário administrador e atualizar a página, a aplicação passou a reconhecer a modificação.

Com isso, a mensagem exibida foi alterada para:

> Cookie Monster 🍪
>
> NOM NOM NOM! DELÍCIA! Aqui está sua flag: FLAG{C00K1E_M0NST3R_MUNCH}

O resultado da alteração pode ser observado na figura abaixo:

![Flag Obtida](https://github.com/LucasBarros29/Write_Up/blob/main/Imagens/cookie02.png)

## 🚩 Flag

```text
FLAG{C00K1E_M0NST3R_MUNCH}
```

## 📚 Conclusão

Este desafio demonstra uma vulnerabilidade comum em aplicações web: confiar em informações armazenadas no lado do cliente para controlar permissões de acesso.

A atividade reforça a importância de inspecionar cookies durante análises de segurança e evidencia por que validações críticas devem ser realizadas pelo servidor, e não apenas pelo navegador do usuário.

Além disso, o desafio mostra como ferramentas simples presentes nos navegadores podem ser extremamente úteis para identificar falhas e compreender o funcionamento de aplicações web.
