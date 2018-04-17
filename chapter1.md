# Como aplicar o estilo

Existem algumas maneira de aplicar o estilo em uma página HTML. A forma mais simples é a aplicação direto na tag do elemento que deseja-se formatar. Essa maneira é conhecida como _inline_.

```html
<p style="color: red;"> Timão e Pumba a dupla que é demais! </p>
```

A figura abaixo apresenta o resultado obtido através da formatação:

![](/assets/inline-formatacao.png)

Outra maneira de aplicar a formatação em uma página HTML é utilizando a tag **style** dentro da head. Essa aplicação de estilo é conhecida como _estilos internos_.

```html
<html>
    <head>
        <title>Exemplos de Estilo com CSS</title>
        <style>
            p {
                color: lime;
            }
        </style>
    </head>
    <body>
        <p>Leia e Han Solo são o casal mais sensacional do universo!</p>
    </body>
</html>
```

Confira o resultado que obtem-se com esse código:

![](/assets/internal-estilo.png)

Ainda pode-se criar um arquivo de estilo para que a formatação criada seja aproveitada em diversas páginas. Essa é uma aplicação de _estilo externa_. O primeiro passo é criar um arquivo com a extensão css. Seu conteúdo é o mesmo que é inserido entre as tags **&lt;style&gt; ... &lt;/style&gt;**.

```css
p {
    color: navy;
}
```

E depois se insere o arquivo através de um link, dentro do arquivo html que deseja utilizar o estilo.

```html
<html>
<head>
    <title>Exemplos de Estilo com CSS</title>
    <link rel="stylesheet" type="text/css" href="estilo.css" />
</head>
<body>
    <p>Leia e Han Solo são o casal mais sensacional do universo!</p>
</body>
</html>
```

Veja o resultado:

![](/assets/estilo-externo.png)

Nessa apostila, por questões didáticas, será adodato o uso da aplicação de estilo interna.

