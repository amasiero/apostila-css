# Texto

Nesse capítulo é apresentado os principais estilos para formatar os textos em uma página HTML.

## Fonte

Existem várias propriedades que auxiliam na formatação das fontes do texto que é exibido na página HTML. As propriedades principais são:

* font-size: determinar o tamanho da fonte. Pode ser informado através de um número em pixels, ou literal, de acordo com a lista abaixo:
  * medium
  * xx-small
  * x-small
  * small
  * large
  * x-large
  * xx-large
  * smaller
  * larger
* font-family: determinar qual fonte deve ser aplicada no texto. Essas fontes devem ser instaladas no computador do cliente. Pode-se determinar o valor de uma fonte em específico, como "Arial" , "Times", "Verdana", "Helvetica", entre outras. Ou de uma maneira mais genérica com as opções: "serif", "sans-serif", "cursive", "fantasy", "monospace".
* font-weight: determinar a largura da fonte \(negrito\). Ela aceita as seguintes opções: normal, bold, bolder, lighter.
* font-style: determinar o estilo da fonte \(itálico\). Ela aceita as seguintes opções: normal, italic, oblique.

* font: é um atalho para utilizar as propriedades acima.

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">
        #size {
            font-size: 20px;
        }

        #family {
            font-family: Helvetica, Arial, Sans-Serif;
        }

        #weight {
            font-weight: bolder;
        }

        #style {
            font-style: italic;
        }

        #shorthand {
            font: italic bold 12px Verdana, Arial, Helvetica;
        }
    </style>
</head>
<body>
    <p id="size">Star Wars</p>
    <p id="family">É a história mais incrível que já existiu! Desculpa Batman!</p>
    <p id="weight">E ainda tem personagens completos, com diversas características legais.</p>
    <p id="style">Leia e Han Solo são o casal mais sensacional do universo!</p>
    <p id="shorthand">Mas não esqueça do Chewie! Arrrrghhhhhh!!!!</p>
</body>
</html>
```

Resultado:

![](/assets/fonts.png)

Caso seja uma opção utilizar uma família de fonte que não esteja instalada no computador do cliente, é possível informar o arquivo de uma família de fonte armazenada no servidor e fazer com que o navegador utilize ela. Porém, cuidado com  o tipo de fonte, pois não são todas suportadas nos navegadores.

Para criar a família de fonte é utilizado o comando **@font-face** e depois basta associar com o nome aplicado através da propriedade **font-family**. Veja o exemplo:

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">
        @font-face {
            family: "Roboto";
            src: url(Roboto-Regular.ttf);
        }

        div {
            font-family: Roboto;
        }
    </style>
</head>
<body>
    <div>
        <h1>Star Wars</h1>
        <p>É a história mais incrível que já existiu! Desculpa Batman!</p>
        <p>E ainda tem personagens completos, com diversas características legais.</p>
        <p>Leia e Han Solo são o casal mais sensacional do universo!</p>
        <p>Mas não esqueça do Chewie! Arrrrghhhhhh!!!!</p>
    </div>
</body>
</html>
```

Tem-se o seguinte resultado:

![](/assets/font-face.png)

## Propriedades do texto

A primeira propriedade que é apresentada referente a textos em geral tem como objetivo trabalhar o alinhamento do texto. Essa propriedade é o **text-align** e ela pode receber os seguintes valores: left \(alinhado à esquerda\), right \(alinhado à direita\), center \(centralizado\) e justify \(alinhado de maneira onde os textos tem a mesma proporção entre as linhas\). Veja o exemplo:

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">
        p.a {
            text-align: left;
        }

        p.b {
            text-align: right;
        }

        p.c {
            text-align: center;
        }

        p.d {
            text-align: justify;
        }
    </style>
</head>
<body>
    <div>
        <h1>Star Wars</h1>
        <p class="a">É a história mais incrível que já existiu! Desculpa Batman!</p>
        <p class="b">E ainda tem personagens completos, com diversas características legais.</p>
        <p class="c">Leia e Han Solo são o casal mais sensacional do universo!</p>
        <p class="d">Mas não esqueça do Chewie! Arrrrghhhhhh!!!!</p>
    </div>
</body>
</html>
```

Resultado:![](/assets/text-align.png)

Outra propriedade existem para textos são decorações como sublinhado, linhas acima do texto ou até mesmo em cima do texto. Essa propriedade é chamada de **text-decoration**. Os valores esperados por essa propriedade são: underline \(sublinhado\), overline \(linha acima do texto\) e line-through \(texto riscado\). Esses valores também podem ser combinados gerando novos tipos de decorações. Confira o exemplo abaixo:

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">
        p.a {
            text-decoration: underline;
        }

        p.b {
            text-decoration: overline;
        }

        p.c {
            text-decoration: line-through;
        }

        p.d {
            text-decoration: underline overline line-through;
        }
    </style>
</head>
<body>
    <div>
        <h1>Star Wars</h1>
        <p class="a">É a história mais incrível que já existiu! Desculpa Batman!</p>
        <p class="b">E ainda tem personagens completos, com diversas características legais.</p>
        <p class="c">Leia e Han Solo são o casal mais sensacional do universo!</p>
        <p class="d">Mas não esqueça do Chewie! Arrrrghhhhhh!!!!</p>
    </div>
</body>
</html>
```

Resultado:

![](/assets/text-decoration.png)

Pode-se ainda definir o tipo de linha e a cor da linha na propriedade do **text-decoration**. Veja o exemplo:

```css
p.a {
        text-decoration: underline red dashed;
}
```

Resultado:

![](/assets/text-decoration-full.png)

