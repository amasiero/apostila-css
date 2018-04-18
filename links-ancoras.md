# Links Âncoras

Os elementos de link âncora promovem a navegação de uma página, seja interna ou externamente. Dessa maneira, como retorno positivo para o usuário, esses elementos possuem pseudo classes que auxiliam no _feedback_ ao usuário. Essas pseudo classes são o próprio link \(**link**\), um link visitado \(**visited**\) e quando o ponteiro do mouse está sobre o link \(**hover**\). Assim, durante a aplicação de um estilo pode-se alterar cada uma dessas pseudo classes, conforme desejado. Veja o exemplo dos links antes da aplicação de estilo:

```html
<body>
    <div>
        <p><a href="#linha1">Ir linha 1</a> | <a href="#linha2">Ir linha 2</a> | <a href="#linha3">Ir linha 3</a> | <a href="#linha4">Ir linha 4</a></p> 
        <h1>Star Wars</h1>
        <p id="linha1">É a história mais incrível que já existiu! Desculpa Batman!</p>
        <p id="linha2">E ainda tem personagens completos, com diversas características legais.</p>
        <p id="linha3">Leia e Han Solo são o casal mais sensacional do universo!</p>
        <p id="linha4">Mas não esqueça do Chewie! Arrrrghhhhhh!!!!</p>
    </div>
</body>
```

Resultado:

![](/assets/link-antes.png)

Perceba que o linha "Ir linha 2" já foi visitado. Nesse caso ele apenas troca a cor do texto. A pseudo classe hover apenas troca a figura do ponteiro do mouse. Agora, veja o código que torna possível a manipulação de cada uma das pseudo classes:

```html
<style type="text/css">
    a:link {
        text-decoration: none; 
    }

    a:visited {
        color: red;
    }

    a:hover {
        text-transform: uppercase;
        text-decoration: underline;
    }
</style>
```

Resultado:

![](/assets/links-formatados.png)

Agora o efeito da pseudo classe hover é mais perceptível, pois a formatação do estilo aplicado foi alterado \("Ir linha 4"\). Assim, é possível criar até formatação de botões para cada um dos links âncoras utilizados na página.

