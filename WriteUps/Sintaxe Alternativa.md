# 🧠 Brainfuck Decoder

> 📂 Categoria: Criptografia

## 🎯 Introdução

Este desafio aborda conceitos básicos de criptografia e linguagens esotéricas. O objetivo é analisar um código escrito em Brainfuck e descobrir a mensagem oculta produzida por sua execução.

## 🔍 Análise Inicial

O desafio fornecia apenas o seguinte código:

```brainfuck
+++++++[<++++++++++>-]<.[-]>+++++++[<++++++++++>-]<++++++.[-]>++++++[<++++++++++>-]<+++++.[-]>+++++++[<++++++++++>-]<+.[-]>++++++++++++[<++++++++++>-]<+++.[-]>+++++++++[<++++++++++>-]<+++++++++.[-]>++++[<++++++++++>-]<++++++++.[-]>++++++++++[<++++++++++>-]<.[-]>++++[<++++++++++>-]<+++++++++.[-]>++++++++++[<++++++++++>-]<+++.[-]>++++[<++++++++++>-]<++++++++.[-]>+++++++++[<++++++++++>-]<+++++.[-]>+++++[<++++++++++>-]<+.[-]>+++++++++++[<++++++++++>-]<+++++.[-]>++++[<++++++++++>-]<++++++++.[-]>+++++++++++[<++++++++++>-]<++++++.[-]>+++++[<++++++++++>-]<+.[-]>+++++++++++[<++++++++++>-]<++++.[-]>++++[<++++++++++>-]<+++++++++.[-]>+++++++++[<++++++++++>-]<+++++++++.[-]>++++[<++++++++++>-]<++++++++.[-]>++++++++++++[<++++++++++>-]<+++++.
```

À primeira vista, a sequência de símbolos pode parecer aleatória. Entretanto, os caracteres utilizados (`+`, `-`, `<`, `>`, `[`, `]` e `.`) são característicos da linguagem Brainfuck.

## 💡 Interpretação

Brainfuck é uma linguagem de programação esotérica criada para ser extremamente minimalista. Ela possui apenas oito comandos e manipula valores armazenados em células de memória.

Ao identificar que o código estava escrito nessa linguagem, a principal hipótese foi executá-lo em um interpretador Brainfuck para descobrir a mensagem produzida.

## ⚙️ Resolução

Para validar a hipótese, o código foi inserido em um interpretador Brainfuck online.

Após a execução, o programa revelou a seguinte mensagem:

```text
FLAG{c0d1g0_3s0t3r1c0}
```

Dessa forma, a flag foi obtida diretamente a partir da saída gerada pelo programa.

## 🚩 Flag

```text
FLAG{c0d1g0_3s0t3r1c0}
```

## 📚 Conclusão

Este desafio introduz o conceito de linguagens esotéricas, em especial o Brainfuck. A atividade demonstra a importância de reconhecer padrões e identificar tecnologias específicas antes de tentar soluções mais complexas.

Muitas vezes, compreender a natureza dos dados fornecidos é suficiente para encontrar o caminho correto para a resolução do desafio.
