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

Existe também a possibilidade de aplicar um estilo diferente para cada borda do elemento. A seguir, é demonstrado o código para aplicação dos 4 principais estilos de bordas.

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">
        p#linha1 {
            border-style: dotted;
        }

        p#linha2 {
            border-style: dashed;
        }

        p#linha3 {
            border-style: solid;
        }

        p#linha4 {
            border-style: double;
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

Confira o resultado:

![](/assets/border-style.png)

Para alterar a cor da borda é necessário utilizar a propriedade **border-color**. Ela funciona da mesma maneira que a cor para o texto. Pode-se utilizar o nome da cor de maneira literal \(em inglês\) e também a aplicação de valores em hexadecimal. Veja o exemplo:

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">
        p#linha1 {
            border-style: solid;
            border-color: red;
        }

        p#linha2 {
            border-style: solid;
            border-color: #a32200
        }

        p#linha3 {
            border-style: solid;
            border-color: #888;
        }
    </style>
</head>
<body>
    <div>
        <p id="linha1">É a história mais incrível que já existiu! Desculpa Batman!</p>
        <p id="linha2">E ainda tem personagens completos, com diversas características legais.</p>
        <p id="linha3">Leia e Han Solo são o casal mais sensacional do universo!</p>
    </div>
</body>
</html>
```

Resultado obtido:

![](/assets/border-color.png)

Por fim, a propriedade de arredondar os cantos é a **border-radius**. Nessa propriedade são informados 4 parâmetros. Da esquerda para a direita os significados são: superior esquerdo, superior direito, inferior direito e inferior esquerdo. Os parâmetros podem ser determinados de acordo com as unidades de medidas existentes, como por exemplo, px, pt, cm, em, etc. A seguir o código para exemplificar a propriedade **border-radius**:

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">
        p#linha1 {
            border-style: solid;
            border-radius: 5px 5px 5px 5px;
        }

        p#linha2 {
            border-style: solid;
            border-radius: 15px 15px 15px 15px;
        }
    </style>
</head>
<body>
    <div>
        <p id="linha1">É a história mais incrível que já existiu! Desculpa Batman!</p>
        <p id="linha2">E ainda tem personagens completos, com diversas características legais.</p>
    </div>
</body>
</html>
```

Este é o resultado no navegador:

![](/assets/border-radius.png)

## Margin e Padding

Margin é a propriedade que define a distância entre as bordas externas do elemento e os demais integrantes da página. Ela pode ser trabalha de maneira unificida através da propriedade ** margin** ou de maneira individual com as propriedades: **margin-top, margin-right, margin-bottom **e **margin-left**. Ao utilizar de maneira unificada, a sequência dos parâmetros informada deve ser: topo, direita, embaixo e esquerda. A seguir, um exemplo de configuração de margin:

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">
        p{width: 500px;}
        p#linha1 {
            border-style: solid;
            border-color: darkgreen;
            border-radius: 5px 5px 5px 5px;
            background-color: lightgreen;
            margin: 60px 10px 40px 50px;
        }

        p#linha2 {
            border-style: solid;
            border-radius: 5px 5px 5px 5px;
        }
    </style>
</head>
<body>
    <div>
        <h1> Star Wars </h1>
        <p id="linha1">É a história mais incrível que já existiu! Desculpa Batman!</p>
        <p id="linha2">E ainda tem personagens completos, com diversas características legais.</p>
    </div>
</body>
</html>
```

O resultado é:

![](/assets/margin.png)

O elemento em verde está com as margins configuradas para exemplificar a diferença na configuração da distância entre os elementos.

O padding segue o mesmo princípio e definições da margin para trabalhar com a propriedade no código CSS. A diferença é que o padding trabalha com a borda interna do elemento. É a distância entre o conteúdo do elemento e seus limites. O exemplo abaixo demonstra uma configuração de paddings entre dois parágrafos.

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">
        p{width: 500px;}
        p#linha1 {
            border-style: solid;
            border-color: darkgreen;
            border-radius: 5px 5px 5px 5px;
            background-color: lightgreen;
        }

        p#linha2 {
            border-color: darkred;
            border-style: solid;
            border-radius: 5px 5px 5px 5px;
            background-color: salmon;
            padding: 20px 20px 20px 20px;
        }
    </style>
</head>
<body>
    <div>
        <p id="linha1">É a história mais incrível que já existiu! Desculpa Batman!</p>
        <p id="linha2">E ainda tem personagens completos, com diversas características legais.</p>
    </div>
</body>
</html>
```



