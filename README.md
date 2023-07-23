# ❄️ Repositório: Como modificar e personalizar o cursor

<div align="center">
<img src="https://i.imgur.com/G7LYPig.gif" alt="CursorGif" />
<div / >

Muitos amigos me pediram para ensinar como personalizar e animar o cursor de um projeto ou site. Por esse motivo decidi fazer esse repositório para eles e a quem mais desejar aprender esse simples processo de modificar o cursor como bem entender. 

- Primeiramente vou explicar a lógica por trás de como funciona a aplicação e como faremos.
- Deixarei o projeto nesse repositório, caso desejarem, podem copiar a vontade ou modificá-lo para atender suas necessidades.
- Vale dizer que esse projeto foi feito usando apenas JavaScript, CSS e HTML, sem nenhuma biblioteca externa. E funciona perfeitamente em React, Angular etc.

~~~javascript
 A lógica se consiste em fazer um container, seja uma div, uma imagem ou seja o que for para ser seu cursor ->
 Depois o modificamos e estilizamos. ->
 Para ele se mexer usamos um simples algoritimo de JS, um eventlistener do mousemove ou seja ele ativa cada vez que seu mouse se mexe. ->
 Esse event listener, vamos pegar uma das caracteristicas que ele vai devolver, a localização X e Y do posicionamento exato do seu cursor na tela. ->
 com isso, usamos o Js para mudar a .style.top e .style.left da div ( nosso cursor ) para a posição exata do nosso mouse ->
 Então, nossa div sempre estará na mesma posição do nosso mouse, mas muita atenção, antes é necessário fazer algumas alterações no CSS da nossa div como por exemplo adicionar uma Position: fixed para ele poder se mover livremente pela tela. ->
 Após feita essas modificações no CSS, uma ultima modificação é necessária, no css body ou * , adicionar cursor: none para esconder seu cursor nativo. ->
 Outras modificações são necessárias para melhor funcionamento, como fazer uma função para esconder o cursor caso ele saia da tela, mas fique tranquilo que explicarei tudo no passo a passo!
~~~

1 Passo: Vamos criar um container, nesse caso uma Div para ser nosso cursor. ( Pode ser também uma imagem. )
⬇️
2 Passo: Vamos personalizar esse container 


