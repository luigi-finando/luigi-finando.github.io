---
layout: post
title:  "Jekyll e o _markdown_"
date:   2017-12-22 15:35:00 -0200
author: Luís
comments: true
category: blog
---

[Markdown]:https://daringfireball.net/projects/markdown/
[Jekyll]:https://jekyllrb.com/docs/home
[Liquid]:https://shopify.github.io/liquid/
[YAML]:yaml.org
[RubyGem]:https://en.wikipedia.org/wiki/RubyGems
[GithubPages]:https://pages.github.com
[Github]:https://www.github.com
[MeuGithub]:https://www.github.com/luigi-finando

## Sobre o *markdown*

[Markdown][Markdown] é uma *markup language* como *html* e *LaTeX*, ou seja, a escrita ocorre primeiramente em formato *plain text*. A formatação se dá a partir de marcações convencionadas, quando o código-fonte é compilado.

A convenção para a criação de um parágrafo é deixar uma linha em branco, por exemplo. A fonte destes mesmos parágrafos tem a seguinte aparência:

```plain-text
[Markdown][Markdown] é uma *markup language*, ou seja, como *html* e *LaTeX*, ela exige que a escrita do texto seja em formato *plain text*. A formatação em si ocorre a partir de marcações convencionadas, quando o código-fonte é compilado em um estágio posterior.

A convenção para a criação de um parágrafo é deixar uma linha em branco, por exemplo. A fonte destes mesmos parágrafos tem a seguinte aparência:
```

Títulos são criados usando o sinal ` # ` e subtítulos são iterações do mesmo sinal repetido, com os subníveis crescendo na mesma medida: 
```plain-text
## Subtítulo
```

> ## Subtítulo

```
### Subsubtítulo
```
> ### Subsubtítulo

Marcações como **negrito** e *itálico* são possíveis com o uso de arteriscos, e a versão do `markdown` oferecida pelo Github ainda permite o texto ~~tachado~~.

## A plataforma [Jekyll][Jekyll] e o [Github Pages][GithubPages]

Essa plataforma, instalada como uma [Ruby Gem][RubyGem], é uma combinação de [Liquid][Liquid] e [Markdown][Markdown], sendo uma ferramenta para a geração de *websites* estáticos.

A integração com *markdown* é essencial pois permite que a sintaxe Liquid e o uso de *Frontmatters [YAML][YAML]* automatizem a geração de *htmls* a partir de templates e pedaços de código. 

Ao executar `jekyll new [nome da página]`, Jekyll produz um ambiente de desenvolvimento com uma estrutura de pastas e o arquivo `_config.yml`, permitindo ao usuário inserir criar layout e trechos de HTML reutilizáveis por meio da sintaxe *Liquid*. Como qualquer documento em HTML, é possível que o usuário crie estilos no formato CSS. A pasta `_posts` aceita arquivos no formato *markdown*, convertendo-os para HTML automaticamente no momento da construção do *site*.

A plataforma [Github Pages][GithubPages] oferece a compilação automática do código do Jekyll, bastando sincronizar os arquivos fonte no repositório. A geração deste *blog* é feita quando o código fonte é enviado ao [meu repositório][MeuGithub] no [Github][Github].
