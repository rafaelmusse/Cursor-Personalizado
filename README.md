# ❄️ Repositório: Como modificar e personalizar o cursor

<div align="center">
<img src="https://i.imgur.com/G7LYPig.gif" alt="CursorGif" />
<div />

🔴   Para ver a aplicação ➡️ [Clique Aqui!](https://rafaelmusse.github.io/Cursor-Personalizado/)   🔴

Muitos amigos me pediram para ensinar como personalizar e animar o cursor de um projeto ou site. Por esse motivo decidi fazer esse repositório para eles e a quem mais desejar aprender esse simples processo de modificar o cursor como bem entender. 

<ul align="left">
<li>Primeiramente vou explicar a lógica por trás de como funciona a aplicação e como faremos.</li>
<li>Deixarei o projeto nesse repositório, caso desejarem, podem copiar a vontade ou modificá-lo para atender suas necessidades.</li>
<li>Vale dizer que esse projeto foi feito usando apenas JavaScript, CSS e HTML, sem nenhuma biblioteca externa. E funciona perfeitamente em React, Angular etc.</li>
<ul />

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
<div align="left">
1 Passo: Vamos criar um container, nesse caso uma Div para ser nosso cursor. ( Pode ser também uma imagem. )
<br />
⬇️
<br />
2 Passo: Vamos personalizar esse container para ser nosso cursor, pode colocar border color e radius para fazer um circulo animado, ou utilizar uma IMG para ser seu cursor. ( Caso deseje, pode copiar um dos que fiz nesse repositorio. ) Lembre-se de colocar Position: Fixed e z-index: 999 ( para o objeto ter prioridade na order de aparecimento na tela. ) no CSS da div.
<br / >
 ⬇️
 <br />
 3 Passo: Vamos criar um Eventlistener de "mousemove" e capturar um dos retornos, o eixo X e Y da posição exata do mouse, e aplicar no .style.top e .style.left de nossa div esse valor. ( Lembrando que a div precisa do atributo -> Position: Fixed, para poder se mover livremente pelos objetos da pagina.
 <br />
 ⬇️
 <br />
 4 Passo: Adicionar o atributo cursor: none; em body ou * no CSS.
 <br />
 ⬇️
 <br />
 Em tese seu cursor estará pronto, porém existem outros mecanismos para melhorar ainda mais sua usabilidade: Função para desabilitar o cursor caso o mouse saia da tela com a propriedade display: none. Ou caso o mouse fique inativo por um determinado periodo de tempo, desabilitar a animação.
</div>


