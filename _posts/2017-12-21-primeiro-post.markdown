---
layout: post
title:  "Jekyll e o *markdown*"
date:   2017-12-22 15:35:00 -0200
author: Luís
comments: true
category: blog
---

## Sobre o *markdown*

`Markdown` é uma *markup language*, ou seja, como *html* e *LaTeX*, ou seja, a escrita do texto ocorre primeiramente em formato *plain text*. A formatação em si se dá a partir de marcações convencionadas, quando o código-fonte é compilado em um estágio posterior.

A convenção para a criação de um parágrafo é deixar uma linha em branco, por exemplo. A fonte destes mesmos parágrafos tem a seguinte aparência:

```plain-text
`Markdown` é uma *markup language*, ou seja, como *html* e *LaTeX*, ela exige que a escrita do texto seja em formato *plain text*. A formatação em si ocorre a partir de marcações convencionadas, quando o código-fonte é compilado em um estágio posterior.

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

## A plataforma Jekyll

Essa plataforma, baseada em Ruby, Liquid e se utilizando do *markdown*, é uma ferramenta para a geração de *websites* estáticos.

A integração com *markdown* é essencial pois permite, juntamente com a sintaxe Liquid e o uso de *Frontmatters YAML* a automatização da geração de html a partir de templates e pedaços de código. A geração deste blog, por exemplo, acontece a partir de funções e *loops* simples.

Uma série de templates e layouts *html*, distribuídos em uma rede de pastas no diretório *root* do site, a partir de um arquivo `_config.yml`, são concatenados com a sintaxe Liquid, e a plataforma Jekyll proporciona a compilação de arquivos `.markdown` para gerar os textos em si.

