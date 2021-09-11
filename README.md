# SVG

O SVG é a abreviatura de Gráficos Vetoriais Escaláveis, ou seja, ele é um tipo de linguagem xml, uma linguagem de marcação, que usa cálculos matemáticos para gerar imagens.

O SVG é um padrão que foi criado em 1998 pelo W3C.

path:

   M = move até
   L = linha até
   H = linha horizontal até
   V = linha vertical até
   C = curva até
   S = curva suave até
   Q = curva de Bézier
   T = curva de Bézier suave
   A = arco elíptico
   Z = fecha path

MAIÚSCULA e minúscula. A versão maiúscula se refere a coordenadas absolutas e a versão minúscula a coordenadas relativas. Por exemplo:

M 100,100 significa Pegue uma caneta e a posicione nas coordenadas exatas 100,100" m 100,100 significa Pegue uma caneta e a posicione 100 para baixo e 100 para a direita a partir da posição em que a sua caneta se encontra agora.

CSS interno
```html
<defs>
  <style>
    .cls-1{fill:#6dbd45;}
    .cls-2{fill:#fff;}
    .cls-3{fill:#f68e49;}
  </style>
</defs>
```

Estilo incorporado
```html
<path d="M265,170.35S367.54,7.18,499,137.48C499,137.48,345.63,117.92,265,170.35Z" style="fill:#6dbd45"/>
```

Atributos de apresentação
```html
<path d="M265,170.35S367.54,7.18,499,137.48C499,137.48,345.63,117.92,265,170.35Z" fill="#6dbd45"/>
```

A propriedade de CSS animation é uma "propriedade abreviada" (ou "shorthand property"), então podemos juntar várias propriedades em uma só, o que economiza linhas e deixa o código mais organizado. São elas:

Animation-name (nome para "chamarmos" a animação)
Animation-duration (duração em segundos ou milissegundos)
Animation-timing-function (controla a velocidade da animação: a mesma durante a animação toda, mais lenta no início, mais lenta no final, etc)
Animation-delay (o tempo de pausa antes de iniciar a animação, em segundos ou milissegundos)
Animation-iteration-count (quantas vezes a animação será reproduzida em sequência)
Animation-direction (a direção da animação: direção normal, de trás para frente, alternando normal e trás para frente, etc)
Animation-fill-mode (podemos aplicar estilos diferentes na animação enquanto ela executa)
Animation-play-state (especifica se a animação está sendo executada ou pausada)

Colocando isso num exemplo:
```
elemento {
  animation: [name] [duration] [timing-function] [delay] [iteration-count] [direction];
}
```
ou

```css
.caiaque {
  animation: marola 5s linear 2s infinite alternate; 
}
```

Lembrando que os valores de viewBox são:

viewBox="[posição eixo X] [posição eixo Y] [tamanho X] [tamanho Y]"

Dessa forma, quando declaramos viewBox="250 0 500 200" para o segundo elemento, estamos posicionando nossa "janela" deslocada em 250px à direita com relação ao vetor (como demonstrado usando a ferramenta Navegador do Illustrator).

Temos a impressão que o quadrado é que andou, mas a janela de visualização é que foi deslocada! Por isso o quadrado aparece "cortado".
