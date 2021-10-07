## Introdução sobre o CSS

O CSS (Cascading Style Sheets ou Folhas de Estilo em Cascata) é uma linguagem de estilo usada para descrever a apresentação de um documento escrito em HTML ou em XML (incluindo várias linguagens em XML como SVG, MathML ou XHTML). O CSS surgiu no ano de 17 de dezembro de 1994, seus criadores foram Håkon e Bert Bos, mas o CSS só veio ganhar sua fama no ano de 1996, quando sua proposta foi aceita na W3C. 

Dois anos depois, no dia 12 de Maio de 1998, eles lançaram a recomendação do CSS de nível 2. A segunda versão do CSS para web. 

O nível 3 do CSS começou seu desenvolvimento em 1999, sua evolução ainda continua até os dias atuais, chegando na versão CSS3 level 4. Importante destacarmos que o ciclo do CSS está proposto a chegar até o CSS3, não haverá CSS4, e sim algo do tipo: CSS3 level 4, CSS3 level 5 e etc..

## Estrutura do CSS

Para trabalharmos com CSS precisamos a seguinte estrutura:

```Estruutura css

/* este é um comentário css */
seletor [, seletor2, ...][:pseudo-classe] {
  propiedade: valor;
}

```

Uma instrução CSS consiste de um seletor, bloco de declaração. Cada declaração contém uma propriedade e um valor, separados por dois pontos (:). Cada declaração é separada por ponto e vírgula (;), não é muito complicado de entender srsrsr... Abaixo uma explicação separada sobre seletores, pseudo classes, propriedades e valores 

### Seletores

Os seletores são usados para declarar a quais elementos de marcação o estilo se aplica, uma espécie de expressão correspondente. Os seletores podem ser aplicados a todos os elementos de um tipo específico, ou apenas aqueles elementos que correspondam a um determinado atributo; elementos podem ser combinados, dependendo de como eles são colocados em relação uns aos outros no código de marcação, ou como eles estão aninhados dentro do objeto de documento modelo. 

``` exemplos de seletores
p{} /*Este é de forma direta no elemento*/
.classe{} /*Seletor classe é usado um ponto final + nome da classe, algo como: .minhaclasse, ou outro nome. Sua vantagem é a flexibilidade.*/
#id{} /*o seletor id possui o famoso hashtag, ou, "jogo da velha". Para usar esse seletor, você esecreve o # + nome de sua id, algo como: #minhaid. Sua vantagem é a leitura rápida, mas ao contrário da classe o id não é flexível, tornando assim um seletor de valor único.
```

### Pseudoclasse 

Pseudoclasse é outra forma de especificação usada em CSS para identificar os elementos de marcação, e, em alguns casos, ações específicas de usuário para o qual um bloco de declaração especial se aplica. Um exemplo frequentemente utilizado é o :hover pseudoclasse que se aplica um estilo apenas quando o usuário 'aponta para' o elemento visível, normalmente, mantendo o cursor do mouse sobre ele. Isto é anexado a um seletor como em a:hover ou #elementid:hover. Outras pseudoclasses e pseudoelementos são, p. ex., :first-line, :visited ou :before. Veja abaixo o exemplo.

``` Exemplo de pseudoclasse
/*Ao passar o mouse o texto irá mudar de cor*/
a{
    color: azul;
}
a:hover{
    color: red;
}

```



## Formas de trabalho com CSS 

Podemos trabalhar com CSS inline, na mesma página com a tag style, ou de forma externa. Veremos abaixo esses exemplos.

### CSS inline

O css inline atualmente é pouco utilizado em páginas web, pois, o código fica "poluído" com muita informação, mas não deixa de ser utilizado no desenvolvimento de mailings e e-mail marketing.

Sua utilização é bem simples, para usá-lo, basta inserir o style dentro da própria tag html que ele receberá o efeito. Veja o exemplo abaixo.

```Código html com css inline
<p style="color: blue;">Este é um texto de cor azul</p>
```

Você pode perceber que o texto recebeu o estilo de cor azul, de cara não parece ser algo "poluente", mas ao lotarmos uma página com essa forma, isso complica bastante as manutenções no site.

### CSS na mesma página

Esse tipo de declaração é um pouco diferente da declaração inline, ela é aplicada na mesma página onde estão as tag's a serem estilizadas, o lado positivo é que não precisamos aplicar em cada tag HTML, ficando um pouco mais organizado, mas ainda sim este padrão não é o recomendável. Para trabalhar com essa forma é necessário usar a tag style. Abaixo um exemplo da forma correta.

``` exemplo tag style

<html>
    <head>
        <title>Exemplo de uso tag style</title>
        <style>
            p{
                color: blue;
            }
        </style>
    </head>
    <body>
        <p>Hello World</p>
    </body>
</html>

```

### CSS externo

Como o próprio nome diz, o CSS externo é um arquivo que permiti organizar as responsabilidades entre HTML e CSS, para usar o CSS externo é necessário criar um arquivo de extensão .css, após criado o arquivo você pode importar em seu html com a tag link. Veja o exemplo.

```Exemplo de importação arquivo css
<link href="meuarquivo.css" rel="stylesheet"/>
ou
<link rel="stylesheet" type="text/css" href="meuarquivo.css">
```