#  Localização Cirúrgica

>  Categoria: OSINT / Geolocalização

##  Introdução

Este desafio combina conceitos de OSINT (Open Source Intelligence) e geolocalização. O objetivo era identificar não apenas um monumento conhecido mundialmente, mas determinar a posição exata do fotógrafo utilizando uma combinação de três palavras no formato do serviço What3Words.

##  Análise Inicial

O enunciado do desafio apresentava a seguinte descrição:

> Um monumento conhecido mundialmente pode ser encontrado em segundos. O verdadeiro desafio é descobrir exatamente onde o fotógrafo estava por meio de uma combinação de três palavras.
>
> Formato: FLAG{xxxx.xxxx.xxxx}

A descrição já fornecia uma pista importante: o formato da flag era composto por três palavras separadas por pontos, característica marcante do sistema utilizado pelo What3Words.

A imagem abaixo apresenta o enunciado do desafio:

![Enunciado do desafio](https://github.com/LucasBarros29/Write_Up/blob/main/Imagens/formato-flag.png)

*Figura 1 - Enunciado indicando o formato da flag baseado em três palavras.*

Além disso, foi fornecida uma imagem do local que deveria ser identificado.

![Imagem fornecida pelo desafio](https://github.com/LucasBarros29/Write_Up/blob/main/Imagens/tajmahal.jpg)

*Figura 2 - Fotografia utilizada para a geolocalização.*

##  Interpretação

Ao observar a imagem, foi possível reconhecer rapidamente o monumento como sendo o **Taj Mahal**, localizado em Agra, na Índia.

Entretanto, identificar o monumento não era suficiente para resolver o desafio. O enunciado enfatizava a necessidade de descobrir exatamente onde o fotógrafo estava posicionado.

Outro detalhe importante foi o formato da flag:

```text
FLAG{xxxx.xxxx.xxxx}
```

Esse padrão remete diretamente ao serviço **What3Words**, que divide o mundo em quadrados de 3 metros por 3 metros e atribui a cada um deles uma combinação única de três palavras.

Dessa forma, a principal hipótese foi utilizar o What3Words para localizar precisamente o ponto de onde a fotografia foi tirada.

##  Resolução

Inicialmente foi identificado o Taj Mahal na imagem fornecida. Em seguida, utilizando referências visuais da fotografia, como caminhos, jardins, espelhos d'água e alinhamento do monumento, foi possível aproximar a posição do fotógrafo.

Com o auxílio do What3Words, foram analisados os quadrantes próximos ao ponto exato da captura até encontrar a combinação correspondente.

O resultado obtido pode ser observado na figura abaixo:

![Localização no What3Words](https://github.com/LucasBarros29/Write_Up/blob/main/Imagens/what3words.png)

*Figura 3 - Localização exata identificada através do What3Words.*

A combinação encontrada foi:

```text
commuted.anyway.stutter
```

##  Flag

```text
FLAG{commuted.anyway.stutter}
```

##  Conclusão

Este desafio demonstra como pequenas informações podem ser utilizadas para obter uma localização extremamente precisa. Embora identificar o Taj Mahal tenha sido relativamente simples, o verdadeiro desafio consistia em determinar a posição exata do fotógrafo.

A atividade reforça conceitos importantes de OSINT, análise visual e geolocalização, mostrando como ferramentas abertas como o What3Words podem ser utilizadas para transformar pistas aparentemente simples em informações altamente específicas.

Além disso, o desafio evidencia a importância da observação de detalhes e da interpretação correta do formato solicitado, uma vez que o padrão da flag foi fundamental para direcionar a investigação para a ferramenta adequada.
