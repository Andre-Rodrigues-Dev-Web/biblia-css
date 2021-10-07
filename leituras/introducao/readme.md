## Introdução sobre o CSS

O CSS (Cascading Style Sheets ou Folhas de Estilo em Cascata) é uma linguagem de estilo usada para descrever a apresentação de um documento escrito em HTML ou em XML (incluindo várias linguagens em XML como SVG, MathML ou XHTML). O CSS surgiu no ano de 17 de dezembro de 1994, seus criadores foram Håkon e Bert Bos, mas o CSS só veio ganhar sua fama no ano de 1996, quando sua proposta foi aceita na W3C. 

Dois anos depois, no dia 12 de Maio de 1998, eles lançaram a recomendação do CSS de nível 2. A segunda versão do CSS para web. 

O nível 3 do CSS começou seu desenvolvimento em 1999, sua evolução ainda continua até os dias atuais, chegando na versão CSS3 level 4. Importante destacarmos que o ciclo do CSS está proposto a chegar até o CSS3, não haverá CSS4, e sim algo do tipo: CSS3 level 4, CSS3 level 5 e etc..

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