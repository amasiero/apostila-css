# Elementos Gerais

Nesse capítulo são apresentados formatações que se aplicam em elementos de maneira geral. Todas as propriedades aqui apresentadas podem ser aplicadas em diversos elementos do HTML.

## Bordas

As bordas estão nos limites de todos os elementos do HTML. Podem ser aplicadas as configurações desde o elemento de bloco, como header, section, main, aside, footer e div, até os elementos mais específicos como os inputs e os links âncoras \(&lt;a&gt;\). Pode-se alterar na borda, sua espessura, estilo, cor e ainda se seus cantos serão arredondados ou não.

Para modificar as espessuras das bordas modifica-se a propriedade **border-width** no arquivo CSS. A espessura aceita diferentes unidades de medidas, como por exemplo, px, pt, cm, em, etc. Contudo, caso seja preferência do designer ou programador front-end, é possível utilizar alguns valores pré definidos: thin, medium ou thick.

Segue o exemplo para a propriedade **border-width:**

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">

        p#linha1 {
            border-style: solid;
            border-width: thin; 
        }

        p#linha2 {
            border-style: solid;
            border-width: medium; 
        }

        p#linha3 {
            border-style: solid;
            border-width: thick; 
        }

        p#linha4 {
            border-style: solid;
            border-width: 4px 15px 8px 30px; 
        }

    </style>
</head>
<body>
    <div>
        <h1>Star Wars</h1>
        <p id="linha1">É a história mais incrível que já existiu! Desculpa Batman!</p>
        <p id="linha2">E ainda tem personagens completos, com diversas características legais.</p>
        <p id="linha3">Leia e Han Solo são o casal mais sensacional do universo!</p>
        <p id="linha4">Mas não esqueça do Chewie! Arrrrghhhhhh!!!!</p>
    </div>
</body>
</html>
```

Resultado obtido:

![](/assets/border-width.png)

No código para linha 4, aplicou-se 4 valores na propriedade. Com essa técnica é possível aplicar uma espessura diferente para cada borda. Os parâmetros representam as seguintes bordas : topo, direita, baixo e esquerda.

Além da espessura, é possível alterar também o estilo da borda. Para isso, é necessário alterar os valores da propriedade **border-style**. Essa propriedade tem alguns valores pré definidos:

* dotted : borda pontilhada;

* dashed : borda tracejada;

* solid : borda contínua;

* double : borda contínua dupla;

* groove : borda entalhada;

* ridge : borda rugosa;

* inset : borda intercalar interna;

* outset : borda intercalar externa;

* none : sem borda;

* hidden : borda oculta. 



