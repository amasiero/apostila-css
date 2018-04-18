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





