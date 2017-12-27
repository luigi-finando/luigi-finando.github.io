---
layout: post
date: 2017-12-25 05:00:00 -0200
title: Sobre o VIM
author: Luís
comments: true
categories: rascunho tutoriais blog
---
[vi]:https://pt.wikipedia.org/wiki/Vi
[BramMoolenar]:http://www.moolenaar.net/
[unix]:https://pt.wikipedia.org/wiki/Unix
[goyo]:https://github.com/junegunn/goyo.vim
[limelight]:https://github.com/junegunn/limelight.vim
[limegif]:https://camo.githubusercontent.com/fa4e9321be0b4a565ae84a66bae36e97545c101b/68747470733a2f2f7261772e6769746875622e636f6d2f6a756e6567756e6e2f692f6d61737465722f6c696d656c696768742e676966

# Vim 

*VI IMproved* é uma extensão do [vi][vi] criada pelo programador holandês [Bram Moolenar][BramMoolenar], *vim* não precisa se limitar à programação. 
Escritores, *bloggers*, jornalistas e estudantes fazem uso do programa, havendo uma série de plugins criados para extender sua funcionalidade nesse sentido.
Pessoalmente, utilizo bastante o *vim* como editor LaTeX, tendo extendido o programa com novos atalhos e plugins como [Goyo][goyo] e [Limelight][limelight].

![limegif](https://camo.githubusercontent.com/fa4e9321be0b4a565ae84a66bae36e97545c101b/68747470733a2f2f7261772e6769746875622e636f6d2f6a756e6567756e6e2f692f6d61737465722f6c696d656c696768742e676966)
*Demonstração do limelight no [repositório do desenvolvedor Junegunn][limelight]*


Originalmente criado para o sistema operacional [Unix][unix], *vim* procura seguir a "filosofia" que orientou o desenvolvimento daquele sistema: *cada programa deve cumprir somente uma função e cumpri-la bem*.
Por esse mesmo motivo (e licença por repetir um clichê) *vim* é ao mesmo tempo limitado e poderosíssimo.

Diferente de editores de texto WYSIWYG, *vim* é um editor que trabalha somente com *plain text*.
O programa não é capaz de manipular um texto em sua tipografia, deixando essa função para linguagens *markup* ou outros programas.
Para a redação e edição do texto em si, vim é extremamente eficiente.

Sua relação com computadores mais antigos ainda é responsável por essa eficiência. Tendo em mente um usuário sem mouse, é possível acessar todas as funcionalidades do programa sem afastar as mãos do *home row* do teclado, algo que por si só torna o trabalho com o texto mais rápido. 

Ainda grande parte da eficiência do *vim* é também fruto de sua maior peculiaridade: a modalidade.


# Editor Modal

Os modos do editor estão na colinha abaixo:

>>>
* **normal** - modo padrão, projetado para a movimentação e edição, acessível com `Esc` ou `Ctrl + [`
* **inserção** - modo para escrita em si, acessível com `i`
* **visual** - modo para a seleção visual, ocorrendo por caractere `v`, por linha `V` ou (mais complicado) por bloco `Ctrl + v`
* **comando** - modo da interface do usuário, com `:`


Quando escrevemos com lápis e papel, nunca nos movimentamos pelo texto com o lápis em contato com a página.
Com essa mesma lógica *vim* possui modos diferentes para a redação e para a edição de um texto já escrito.

Ao abrir o programa o usuário o encontra em modo normal, que o modo para movimentação e alteração do texto. Para inserir texto, devemos entra no modo de *inserção*, pressionando a tecla `i`. É nesse modo, e somente nesse modo, que o texto é inserido. Pressionamos `Esc` ou `ctrl + [` para retornarmos ao modo normal.

Toda a interação do usuário com o programa acontece pelo modo de comando, que é acessado pressionando a tecla `:` a partir do modo normal. Comando como sair `:q` ou `:quit`, salvar (*write*) `:w` são passados por meio da linha de comando. Comando mais importante, no entanto, é a ajuda. Ao inserir `:h r`, por exemplo, o programa informa qual a função da tecla r, o mesmo servindo para todas as teclas da *home row* do teclado.

O *vim* ainda apresenta uma série de características interessantes, como a capacidade de concatenar com um sintaxe própria. Pretendo colocar aqui minhas "colinhas" sobre isso.
