# Base de HTML5 para hacking

Documento sobre a linguagem de marcação de construção de páginas é a base para qualquer hacking na web. A importância de conhecimento da base é o início de qualquer carreira na área de segurança, ao contrário de que muitos dizem por aí, saber programar é um pré requisito para o hacking. 

Esse dicionário é apenas um guia sobre tags, por tanto, não é um curso para aprender a desenvolver uma página web.

> HTML é uma Linguagem de Marcação de HiperTexto - Independente do editor de texto utilizado essa linguagem de marcação poderá ser utilizada na construção de páginas de web. 

SAIBA MAIS - Validate de estrutura [W3C](https://validator.w3.org/)

***

 `<!DOCTYPE html>`é a instrução para o browser(navegador) de qual versão do HTML estamos trabalhando.

Os comandos de HTML são utilizados dentro de tags. As tags contém comandos, parâmetros e valores dos parâmetros.

***

```
<html lang="pt-BR">
</html>
```

O `<html` é a tag container raiz/root para todo o contéudo que será trabalhado no projeto. `lang=" "` é o parâmetro que vai indicar a linguagem de todo o projeto, e o que fica dentro de `" "` é o valor desse parâmetro, no caso o idioma português do Brasil `pt-BR` contém símbolos e caracteres que em outras linguagens não são utilizadas, então ao colocar esse valor no parâmetro indicamos que esse projeto irá conter todos os caracteres desse idioma e possibilitará que seja lido pelo browser. 

* Contém fechamento `</html>` 

***

`<head>` Cabeça da página - É o container para outras tags exclusivas que não são visíveis e sim de definições e configurações. 

* Filho de `<html>`
* Contém fechamento `</head>` 

***

`<title>` filha de `<head>` que representa o título da página que é mostrado na barra de título no browser. 

* Filho de `<head>`
* Contém fechamento `</title>`

***

`<body>` Tag Corpo da página. É o container de todos os elementos vísivel da página.

* Filho de `<html>`
* Contém fechamento `</body>`  

***

`<p>` Tag de parágrafo e possui pré configurações. 
* Elemento de fluxo - Elemento que marca o contéudo no corpo da página (visual).  
* Display Block - significa que não aceita um contéudo na mesma linha que ele, automaticamente quebra linha.
* Filho de `<body>`
* Contém fechamento `</p>`

***

`<h1>` 

`<h2>`

`<h3>`

`<h4>`

`<h5>`

`<h6>`
Tags de cabeçalho, ou seja, títulos do conteúdo de texto que será descrito na página. 
* Pré formatação padrão em sistema de hierarquia de níveis   
* Categoria de cabeçalho
* Display: Block 
* Elemento de Fluxo 
* Contém fechamento `</h1> </2> </3> </h4> </h5> </h6>`

Exemplo: 

`<h1>Título de nível 1</h1>`

`<h2>Título de nível 2</h2>`

`<h3>Título de nível 3</h3>`

`<h4>Título de nível 4</h4>`

`<h5>Título de nível 5</h5>`

`<h6>Título de nível 6</h6>` 
# Título de nível 1
## Título de nível 2
### Título de nível 3
#### Título de nível 4
##### Título de nível 5 
###### Título de nível 6

***
`<a>` - Tag âncora - para links e conexões na página web como: arquivos, dowload, áudio, vídeo, imagem, endereços de emails, ligações na mesma página ou endereços na URL.

Todos os elementos que podem ser colocados dentro da tag `<a>`, são parâmetros(pode haver mais de um) de configuração e todo parâmetro deve conter o nome="o valor".

O principal atributo dessa tag *a* é o *href*, que cria uma referência hipertexto. Veja os exemplos abaixo:

`<a href(nome)="seu link aqui(valor)">Texto visível</a>`

Há dois tipos de links durante a construção do seu projeto **link interno** e **link externo**.

`<a href="web2.html"` link local ou interno - documento do seu projeto.

`<a href="https://www.google.com">`link externo - URL commpleta, que inclui o protocolo *http://* ou *https://* construindo o caminho que levará à uma página específica.

`<a href="nome_da_pasta_que_está_o_arquivo_desejado/pagina-dentro-da-pasta.html">Texto visível</a>`- Organização de páginas dentro de pastas na programação do site. Usada para abrir uma pasta(onde está a página a ser aberta) dentro da pasta principal. Pasta sobre pasta. 

`./` Refere-se à pasta atual do servidor.

`../` Refere-se à pasta imediatamente superior. Veja o exemplo:   

`<a href="../nomaedoarquivo.html">Texto visível</a>` - Retornará para a pasta anterior para executar a página desejada.  

O parâmetro target indicará onde o link abrirá de acordo com o valor abriuído à ele, observe os exemplos abaixo :arrow_down:

Substituir a página:
`target="_self"` - mas caso não coloque essa função o hmtl já está pré definido para ler ela automaticamente.

Abrir em uma nova aba:

`target="_blank"`

`<a href="https://github.com/Nandaevangelista" target="_blank">GitHub Nanda</a>`

Abre o documento vinculado ao pai dele:

`target="_parent"`

Abre o documento vincuado ao corpo inteiro da página, ou seja, vai desfazer todos os frames e abrir o destino no navegador completo.

`taret="_top"`


Abre o documento vinculado no iframe nomeado: 

`target="framename"`

*hreflang* permite indicar qual é o idioma principal do site para onde o link está desviando o fluxo de navegação, avisando o browser e softwares de tradução como  traduzir automaticamente os conteúdos. 

`<a href="https://www.google.com" hreflang="en">`


Realiza o **download** de PDF ou arquivo ZIP do valor configurado para o nome do arquivo a ser baixado(arquivo de dentro do seu projeto):

`<a href="nome-da-pasta/arquivo.pdf" download="arquivo.pdf" type="application/pdf"> Baixe aqui o PDF</a>`

**Media types** que podem ser utilizados:

* application/zip
* text/html
* text/css
* text/javascript
* video/mp4
* video/H264
* video/JPEG
* audio/acc
* audio/mpeg
* font/ttf
* image/jpeg
* image/png


**SAIBA MAIS** informações sobre a semântica oferecida pelo [W3C](https://html.spec.whatwg.org/multipage/links.html#linkTypes)
* Contém fechamento `</a>` 

***

`<abbr>` - Abreviações -Mostra um label ao repousar o mouse em cima os caracteres da função 

`<p> Esse é um pequeno dicinário sobre <abbr title="Hypertext Markup Language">HTML</abbr> </p>`

* Display: inline
* Categoria: Fluxo e Fraseado(significa que usa textos no seu interior)
* Atributos: title e [globais](https://www.w3.org/2009/cheatsheet/#inf,html,a,global%20HTML%20attributes)
* Contém fechamento `</abbr>`

*** 

`<address>` Colocando informações de contato apropriada para o contexto, como endereço físico, URL, email, telefone, mídia social, coordenadas geográficas de pessoas físicas ou empresas.

##

```
   <address>
       Autor: W3C<br>
       Informações direto do <a href="https://www.w3c.br" target="_blank">site oficial</a>
   </address>
 ```
 
> *Autor: W3C*
>
> *Informações direto do [site oficial](https://www.w3c.br).*
   
##

* Display: Block
* Cateboria: Fluxo
* Atributos: globais 
* Contém fechamento `</address>`

***

`<article>` Representa uma composição de seção independente em um documento, página, aplicação, ou site, ou que é destinado a ser distribuido de forma independente ou reutilizável. Pode haver quantas tags *article* for necessário, cada uma representando uma área e assunto específico no documento, de conteúdos diferentes de cabeçalho, contéudo ou rodapé. 


```
<article>
   <h1>HTML para Hacking</h1>
   <p>Guia de base para hacking na web.</p> 
</article>
```

* Display: Block
* Categoria: Fluxo e Seção(área da página)
* Atributos: Globais
* Contém fechamento `</article>`

***

`<aside>` representa uma seção de uma página que consiste de conteúdo que é tangencialmente relacionado ao conteúdo do seu entorno, que poderia ser considerado separado do conteúdo principal. Essas seções são, muitas vezes, representadas como barras laterais. Elas muitas vezes contem explicações laterais, como a definição de um glossário; conteúdo vagamente relacionado, como avisos; a biografia do autor; ou, em aplicações web, informações de perfil ou links de blogs relacionados, agrupamento de publicidade, grupos e blocos de navegação e para qualquer outro conteúdo que é separado do conteúdo principal.

Observação: não necessáriamente precisa estar na lateral na página, podendo incluir elementos de fluxo dentro dele como *atributos globais*.

O elemento *aside* pode ir também dentro de um elemento *article* como uma caixa de notação ou algo do genêro. Nesse caso, quando o usuário printar, haverá ênfase a esta caixa como se fosse um box de informação.

* Para a formatação é necessário conhecimento em CSS3
* Display: Block
* Categoria: Fluxo e Seção 
* Atributos: Globais
* Contém fechamento `</aside>`

***

`<audio>` Tag para inserir compenentes de áudio.

`<audio src"seuaudio.mp3" autoplay controls loop></audio>

* Display: None
* Categoria: Fluxo, fraseado e incorporado.
* Atributos: Globais; autoplay; preload; controls; loop; mediagroup;muted; src;
* Contém fechamento `</audio>`

***

`<b>` Formatação em **negrito** - Trabalha diretamente no texto dando destaque à determinados elementos.

`<p>Para o hacking é <b>importante</b> que você conheça a <b>linguagem de marcação html</b>`

* Display: inline
* Categoria: Fluxo e Fraseado
* Contém fechamento `</b>`

***

