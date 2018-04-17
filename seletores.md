# Seletores do CSS

Uma definição para seletores em CSS são todos os elementos que geram alguma saída para o usuário de uma página. Esses elementos são encontrados no geral, através das tags do HTML. Sendo assim, a estrutura de arquivo CSS segue o seguinte formato:

```css
seletor {
    atributo : valor;
}
```

Por exemplo, para formatar um seletor **div** que existe em uma página HTML faz-se o seguinte código.

```css
div {
    background-color: lightgrey;
    border-radius: 5px;
    padding: 20px;
    margin: 0 30px;
}
```

Porém, não é apenas com o uso dos seletores dados através dos nomes das tags que utiliza-se no CSS. Existem outras duas maneiras que pode-se aplicar estilo nos elementos da página. Pode-se aplicar através de uma identificação, utilizando o carácter  da cerquilha ou hashtag \(\#\) ou também com uma classe através do carácter ponto \(.\).

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">
        .azul {
            color : blue;
        }
        #titulo {
            color : red;
        }
    </style>
</head>
<body>
    <div>
        <h1 id="titulo">Star Wars</h1>
        <p class="azul">Leia e Han Solo são o casal mais sensacional do universo!</p>
    </div>
</body>
</html>
```

Confira o resultado:

![](/assets/id-class.png)

Com o uso de classes e identificadores torna-se mais fácil reaproveitar e aplicar estilo em pequenas partes da página ou elementos específicos. Uma outra forma de aproveitar a formatação do estilo é aplicá-la em grupo de seletores. Para isso, basta separar os seletores através de uma vírgula \(,\).

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">
        p, h1 {
            color : darkblue;
        }
    </style>
</head>
<body>
    <div>
        <h1>Star Wars</h1>
        <p>Leia e Han Solo são o casal mais sensacional do universo!</p>
    </div>
</body>
</html>
```

O seguinte resultado é apresentado:

![](/assets/grupo-seletores.png)

Além disso, é possível criar uma hieraquia de seletores, por exemplo, formatar apenas os parágrafos \(&lt;p&gt;\) que estão dentro de uma div com identificador específico. Veja o exemplo:

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <style type="text/css">
        #formatado {
            width: 400px;
            background-color: lightgrey;
            padding: 20px;
        }

        #formatado p {
            color : navy;
        }

        p {
            color : blue;
        }
    </style>
</head>
<body>
    <h1>Star Wars</h1>
    <p>É a história mais incrível que já existiu! Desculpa Batman!</p>
    <div id="formatado">
        <p>E ainda tem personagens completos, com diversas características legais.</p>
        <p>Leia e Han Solo são o casal mais sensacional do universo!</p>
    </div>
</body>
</html>
```

Confira o resultado da formatação:

![](/assets/hierarquia-seletores.png)





