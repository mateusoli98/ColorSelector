### Color Selector


 > Este projeto apresenta uma solução simples para capturar cores em hexadecimal utilizando apenas _HTML, CSS e JavaScript._
 
 ![color-selector](https://user-images.githubusercontent.com/39521693/85173596-f9b58100-b249-11ea-8eed-a2ccf6f5dc23.png)

1. O elemento utlizado para captura de cor foi o input do tipo color nativo do HTML

```
 <input type="color">
 
```
2. Para que o JavaScript possa ser assionado e seja efetiva a troca de cor em tempo real, é necessário utilizar o event _oninput_ chamando uma funcão. Desta forma:

```
<input type="color" oninput="changeColor(this.value)">
```

3. Função _changeColor()_ para setar o background na div receptora da cor selecionada e realizar a troca do texto referente ao valor da cor.

```
function changeColor(color) {
    document.getElementById("resultColor").style.backgroundColor = color;
    document.getElementById("resultvalue").innerText = color;
}

```
