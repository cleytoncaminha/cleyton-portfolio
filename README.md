# Portfólio

## Animação de rotação dos efeitos 

Foi criada uma animação chamada spin que rotaciona os elementos

Primeiro precisamos criar a animação:

0% - inicia no 0 com nenhuma rotação

100% - vai ate o fim da animação rotacionando 360 graus

```css
@keyframes spin {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
```
E depois usamos a animação no elemento que queremos animar

```css
animation: spin 10s linear infinite;
```

spin - nome da animação que criamos 

10s - tempo da animação

linear - a animação vai ter a mesma velocidade do começo ao fim 

infinite - a animação não termina

```css
.effect-purple-square {
  width: 30px;
  height: 30px;
  border: 4px solid #8a49ff;
  right: 10%;
  bottom: 0;
  animation: spin 10s linear infinite;
}

@keyframes spin {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
```

## Animação simples de botão com sombra

[Botão no CodePen](https://codepen.io/kadoohd/pen/ZEyYMRR)

## Fontes responsivas usando rem

Foi utilizada a técnica de diminuir a fonte geral do html pra 62.5% do tamanho padrão.

62.5% de 16px = 10px

E no body é setado um tamanho de fonte de 1.6rem.

Assim toda as fontes podem ser criadas sem a ncessidade de calcular o rem em relação ao pixel.

```css
font-size: 1.6rem;
```

## Diferenças entre width e max-width

Adicionado max-width no container pra restringir o crescimento do container

Se a tela for maior que 1140px ele seta esse valor máximo pro container, se for menor pega 100%
do tamanho