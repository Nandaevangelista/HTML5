# Base de HTML5 para hacking

Documento sobre a linguagem de marcação de construção de páginas é a base para qualquer hacking na web. A importância de conhecimento da base é o início de qualquer carreira na área de segurança, ao contrário de que muitos dizem por aí, saber programar é um pré requisito para o hacking. 

Esse dicionário é apenas um guia sobre tags, por tanto, não é um curso para aprender a desenvolver uma página web.

> HTML é uma Linguagem de Marcação de HiperTexto - Independente do editor de texto utilizado essa linguagem de marcação poderá ser utilizada na construção de páginas de web. 

SAIBA MAIS - Validate de estrutura [W3C](https://validator.w3.org/)

***

<a name="ancora"></a>
# TAGS POR LETRA
- [Tags iniciais](#ancoraPRINCIPAL)
- [A](#ancoraA)
- [B](#ancoraB)
- [C](#ancoraC)
- [D](#ancoraD)
- [E](#ancoraE)
- [F](#ancoraF)

- [Formulário](#ancoraformulario)

<a id="ancoraPRINCIPAL"></a>

# Tags base para inicio de projeto

 `<!DOCTYPE html>`é a instrução para o browser(navegador) que estamos trabalhando com a última versão disponível do HTML. Escrita em caixa alta. 
Os comandos de HTML são utilizados dentro de tags. As tags contém comandos, parâmetros e valores dos parâmetros.

* Não contém fechamento

***

```
<html lang="pt-BR">
</html> 
```

O `<html` Tag container raiz/root para todo o contéudo que será renderizado no browser. Ela precisa abrir na primeira linha e seu fechamento fica na última linha. 

`lang=" "` é o parâmetro que vai indicar a linguagem de todo o projeto, e o que fica dentro de `" "` é o valor desse parâmetro, no caso o idioma português do Brasil `pt-BR` contém símbolos e caracteres que em outras linguagens não são utilizadas, então ao colocar esse valor no parâmetro indicamos que esse projeto irá conter todos os caracteres , dessa forma se um usuário que não entende esse idioma, poderá ser traduzido para sua linguagem natal. 

`<html lang="pt-BR">`

* Contém fechamento `</html>` 

***

`<head>` Cabeçalho da página - Responsável por separar as informações que estão sendo passadas parao browser, ou seja, o container para outras tags exclusivas que não são visíveis e sim de definições e configurações. 

* Filho de `<html>`
* Contém fechamento `</head>` 

***

<meta charset="UTF-8"> Responsável para passar informações do *encoding* ao browser sobre os caracteres especiais que a linguagem do projeto contém.

`meta` Passa as informações para o browser.
`charset` Atributo que informa o valor a ser inserido no projeto.
`UTF-8` É o dicionário que contém todos os caracteres de todas as linguagens, inclusive o português do Brasil.

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

<a id="ancoraA"></a>
# A

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

`<audio src"seuaudio.mp3" autoplay controls loop></audio>`

* Display: None
* Categoria: Fluxo, fraseado e incorporado.
* Atributos: Globais; autoplay; preload; controls; loop; mediagroup;muted; src;
* Contém fechamento `</audio>`

***

<a id="ancoraB"></a>
# B

`<b>` Formatação em **negrito** - Trabalha diretamente no texto dando destaque à determinados elementos.

`<p>Para o hacking é <b>importante</b> que você conheça a <b>linguagem de marcação html</b>.`

> Para o hacking é **importante** que você conheça a **linguagem de marcação html**.

* Display: inline
* Categoria: Fluxo e Fraseado
* Contém fechamento `</b>`

***

`<base>` Facilitador do caminho - Não se utiliza mais do que uma base em um projeto.

```
<base href="arquivo_desejado">
</head>
<body>
<a href="arquivo_da_tag_base">Texto visível</a>
```

* Só pode ser utilizado dentro de *head*
* Display: None
* Categoria: Metadados
* Atributos: Globais; target; hreaf; 
* Não contém fechamento

***

`<bdo>` Direção do texto - Muito utilizado em idiomas que se lê da direita para esquerda como por exemplo o idioma Árabe. 

* ltr - esquerda para a direita.
* rtl - direitapara a esquerda.

`<bdo dir="rtl">Texto que deseja formatar</bdo>`

> ratamrof ajesed euq otxeT

* Display: inline
* Categoria: Fluxo e Fraseaso
* Atributo: Dir
* Contém fechamento `</bdo>`

***

`<blockquote>` Tag de citação de conteúdo externo e  `<cite>` quando aplicado nessa situação vai especificar a origem da origem de *blockquote*. Veja os exemplos abaixo:

```
<blockquote>
<p>Texto extraído de algum autor externo</p>
</blockquote>
```

```
<blockquote cite="url_externa">
<p>Texto extraído de algum autor externo</p>
</blockquote>
```

* Display: Block
* Categoria: Fluxo e Seção 
* Atributos: Globais e *cite*
* Contém fechamento `</blockquote>`

**SAIBA MAIS SOBRE:** `<cite>` - Representa o título de uma obra; referência aos autores; Receberá uma formação específica para a função de citação. 

```
<blockquote>
<p>Texto extraído de algum autor externo.</p>
<cite>Nome do autor</cite>
</blockquote>
```

> *Texto extraído de algum autor externo.*
> 
> *Nome do autor*

* Para melhor formatação é utilizado CSS3
* Display: Inline
* Categoria: Fluxo e fraseado 
* Contém fechamento `</cite>` 

***

`<br>` Tag que representa quebra de linha dentro de endereços e poemas. Não é recomendado uso abusivo dessa *tag* e também mais de um *br* seguido, por exmeplo: `<br><br><br>`. Em casos de formações de textos se utiliza *tags* específicas como `<p>` com display block e formatações de estilo se utiliza o CSS3, que é o responsável exclusivamente para formação de design da página. 

* Display: Inline
* Categoria: Fluxo e fraseado
* Atributos: Globais
* Não contém fechamento 

***

`<button>` Representa um botão clicável pré formatado mas que também pode ser formatado com as preferências do programador através do CSS3(Design) e JavaScript(atribuir ações). 

> Tipos mais comuns em formulários:
>
> Submit: Para indicar os dados à um formulário.
>
> Reset: Limpa os campos do formulário, contém ações pré determinadas
>
> Button - Não tem ações pré determinadas, sendo configuradas em JavaScript

* Display: Inline
* Categoria: Fluxo,fraseado e interativo
* Atributos: Type; Value; Globais;
* Contém fechamento `</button>`

*** 

<a id="ancoraC"></a>
# C

`<canvas>` - Representa uma área(tela de bitmap) que nos permite manipular os desenhos e mapeamento dos elementos. 

* Utiliza JavaScript para ações
* Display: Block
* Categoria: Fluxo, fraseado, incorporado
* Atributos: Globais; widht; height;
* Contém fechamento `</canvas>`

***

`<code>` Apresenta de forma visível e não interpreta como código um texto em código. O seu conteúdo é impresso na tela estilizado de maneira a indicar/destacar que um texto é o fragmento de código dentro do contexto sem renderizar como um código propriamente dito: 

Exemplo impresso: Estamos na *tag* `<code>` - A forma como esse código foi apresentado, será impresso na tela quando utilizar essa tag. 

* A multi-utilização de `<br>` pode ser utilizada.
* Display: Inline
* Categoria: Fluxo e fraseado
* Atributo: Globais
* Contém fechamento `</code>`

***
<a id="ancoraD"></a>
# D

`<del>` Representa um conteúdo que foi excluído ou marcado como eliminado no conteúdo. Formatação de riscado. ~Como nesse exemplo~

Quando aplicado o atributo `<cite>` é para direcionar a url com o motivo que o conteúdo foi deletado.
Quando aplicado o atributo `<datetime>` é para instruir o usuário a data e hora que esse conteúdo foi deletado.

`<del cite="url" datetime="">Texto visível riscado (deletado)</del>`


* Display: Inline-block
* Categorria: Fluxo, contido por fraseado
* Atributos: Cite; Datetime; Globais
* Contém fechamento `</del>`

***

`<details>` e `<summary>` *detaisl* é interativo, usado como uma ferramenta onde o usuário irá obter informações adicionais. *Summary* é filho direto de *Details* - Trabalham em conjunto. Quando o usuário clicar no *título de details* vai **expandir** e mostrar o conteúdo, clicando novamente ele irá **ocultar** o conteúdo. E *summary* é utilizado como um sumário ou legenda para o conteúdo de um elemento *details*.
 
```
<details> 
      <summary>Texto visível</summary>
      <p>Conteúdo que vai aparecer quando for clicado</p>
</details>
``` 

**Details**
* Display: Block
* Categoria: Fluxo; Interativo;
* Atributo: Globais; open;
* Contém fechamento `</details>` e `</summary>` 

***

`<dfn>` Representa uma instância de definição de um termo, ou seja, a representação/abreviação de uma definição. 

```
<p>
   <dfn>HTML</dfn>
   Hypertext Markup Language é uma linguagem de marcação utilizada na construção de páginas na WEB
</p>
```

Usando o atributo title, surgirá um label quando o mouse pousar em cima da abreviação *dfn*.

```
<p>
   <dfn title="Hypertext Markup Language">HTML</dfn>
   É uma linguagem de marcação utilizada na construção de páginas na WEB
</p>
```


* Display: Inline
* Categoria: Fluxo; fraseado;
* Atributo: title; Globais;
* Contém fechamento: `</dfn>` 

***

`<dialog>` Tag para definir uma caixa de diálogo ou outro componente interativo, tal como um inspetor ou janela. 

```
<dialog open>
     Olá Mundo!
</dialog>    
```

* Categoria: Fluxo 
* Atributos: Globais; open;
* Contém fechamento: </dialog>

***

`<div>` Container/complemento de organização para qualquer elemento. Ele pode ser utilizado para agrupar elementos para fins de estilos (usando class ou id).

Exemplo de organização utilizando a tag *div* dentro de um *article* 

##

```
<article>
         <div> 
              <h1>Dicinário html</h1>
                  <p>Guia com definição e utilização das tags por ordem alfabetica.</p>
                  <p>Esse documento é a base para o curso de html para hacking</p>
         </div>
<article>
```

# 1 Dicinário html

Guia com definição e utilização das tags por ordem alfabetica.

Esse documento é a base para o curso de html para hacking

##

* Display: Block
* Categoria: Fluxo
* Atributos: Globais
* Contém fechamento: `</div>`

***

`<dl> <dt> <dd>` Listas de definição - São constituidas de duas partes: um **termo** e uma **descrição**. Para codificar uma lista de definição são necessários três elementos *dl dt dd* trabalham juntas: `<dl>` container(árvore); `<dt>` termo de definição(título); `<dd>` descrição do valor(conteúdo relacionado ao título); 

##

```
<dl> 
    <dt>Dicinário html para hacking</dt
        <dd>Tags com letra - A</dd>
        <dd>Tags com letra - B</dd>
</dl>        
```

##

`<dl>`
* Display: Blcok
* Categoria: Fluxo
* Filhos: `<dt>` e `<dd>` 
* Atributos: Globais
* Contém fechamento: `</dl>`

`<dt>`
* Display: Block
* Categoria: Fluxo
* Contigo por: `<dl>` e `<dialog>`
* Contém fechamento: `</dt>`

`<dd>`
* Display: Block
* Categoria: Fluxo
* Contifo por: `<dl>` e `<dialog>`
* Contém fechamento: `</dd>` 

***

<a id="ancoraE"></a>
# E

 `<em>` Destacar ênfase em um parágrafo. 

`<p>Guia base de <em>html</em> para <em>hacking</em>.</p>`
> Guia base de *html* para *hacking*.


* Display: Inline
* Categoria: Fluxo e fraseado
* Atributos: Globais
* Contém fechamento: `</em>`

***

`<embed>` Representa uma área com ponto de interação de arquivo externo, ou seja, incorporar um conteúdo externo que pode ser interativo.

`<embed src"link_externo">`

* Categoria: Fluxo; Fraseado; Incorporado;
* Atributos: src; type; width; height;
* Não cotém fechamento.

***

<a id="ancoraF"></a>
# F 

`<figure>` Representa um conteúdo de fluxo, uma legenda/container associado à um conteúdo. **OBS:** Não tem relação com imagens como o nome pode acabar sugerindo a associação.

*figcaption* é a legenda do conteúdo *figure* - Identação/organização de projeto em estabelecido. 

```
<figure>
        <p>Guia base de HTML para Hacking</p>
           <figcaption>Dicionário para iniciantes na área de segurança de informação
           </figcaption>
</figure>
```

```
<figure>
        <img src="https://logosmarcas.net/wp-content/uploads/2020/09/Google-Logo.png">
        <figcaption>
           www.google.com
        </figcaption>
</figure>        
```

* Display: Block
* Categoria: Fluxo; Seção;
* Atributos: `<figcaption>`
* Contém fechamento: `</figure>`

***

`<footer>` Tag de seção própria para rodapés do contexto em que ela está inserida, seja da página ou de outras seções.
Exemplos de rodapés de páginas web podem contém muitos elementos diferentes como audio, tabelas, referências e etc. 

* Formatado por CSS
* Display: Block
* Categoria: Fluxo; Seção;
* Atributos: Globais
* Contém fechamento: `</footer>`

***

<a id="ancoraformulario"></a>

## FORMULÁRIO: 

`<form>` Elemento de formuários. Representa uma coleção de elementos de um determinado formulário. Container do formulário. 

``` 
<from name="fcadastro" action="#" method="get">
    <label>Nome:</label> 
       <input type="text" name="fname" 
</from> 
```    

*action* e*method* vão funcionar quando um botão for acionado (usado PHP para isso) 
Quando uma programação *method* é do tipo *get* as informações são direcionadas e gravadas diretamente na URL o que pode causar uma vulnerabilidade, já do tipo *post* pode ser direcionado diretamente impresso na página, mas esse assunto será explicado posteriormente conforme avançamos em hacking. 

* Display: Block
* Categoria: Fluxo
* Atributos: 
  * `<action>` - URL com o arquivo que irá receber o conteúdo do formulario/os dados enviados.
  * `<autocomplete>` - Autocompleta campos ativados.
  * `<enctype>` - Codificação (tipo) dos dados enviados.
  * `<method>`- Método de envio dos dados (get ou post).
  * `<name>` - Nome do formulário.
  * `<novalidade>` - Desabilita a validação pelo browser.
  * `<target>` - Como a página de destino (action) será aberta, se será aberta na página atual ou em um frame específico.
* Contém fechamento: </form>

##

`<label>` Representa uma legenda - Locasl onde o usuário irá preencher - útil no trabalho com formulários. Ela especifica qual o "rótulo" do *input* (a que se refere o input), e ajuda na experiência do usuário durante a utilização e preenchimento do formulário.

* Display: Inline
* Categoria: Fluxo; Fraseado;
* Contém fechamento: `</label>` 

##
 
`<input>`

* Display: Inline
* Categoria: Fluxo; Fraseado; Interativo


   `<type>` Determina o tipo do elemento; Todos abaixo são botões, porém cada um tem um comportamento/função pré definida:
   
    `<input type="text">` - Cria campos de texto básicos em uma linha única.
    
    `<input type="submit">` - Envio dos dados inseridos no formulário (PHP cuidará desses dados, processará e guardar- `method="#"` e `action="#"` serão responsáveis para essa funcionalidade).
    
    `<input type="reset">` - Limpeza dos campos desse formulário.
    
    `<input type="button">` - Elemento que não tem comportamento pré definido, podendo ser manipulado manualmente. 
    
    `<input type="name">` O nome do componente (identificação dos elementos- NÃO VISÍVEL);
    
    `<input type="password>"` - Input para trabalhar com senhas - Quando o conteúdo é digitado ele não fica impresso na tela do usuário. 
    * `input type="password" name="f_senha" pattern="[a-zA-Z0-9]"{12}` Indicará que a senha obrigatoriamente precisa ter `{12}` 12 digitos, sendo caracteres de `[a-z` *a à z* minúsculo, `A-Z` *A à Z* maiúsculo e `0-9]` *0 à 9* números. 
    
    `maxlength="#"` Limitar quantidade de caracteres em senha `maxlength="8"` máximo de 8 caracteres.
    
    `size="#"` Limita visualmente o tamanho da caixa do formulário. 
    
    `<input type="checkbox">` Caixa de seleção que pode ser marcada e desmarcada, podendo selecionar/marcar mais de uma opção.
    
    `<input type="radio">` Caixa de seleção que pode ser marcada ou selecionada por apenas uma opção. 
    
    `<input type="time">` Elemento para trabalhar com horário, ele contém recursos que facilitam a inserção de horário. (Ao acrescentar `<min="#">` e `<max="#">` determinará horario mínimo e máximo de uma determinada função de acordo do que se trata a web).
    
    `<input type="date">` Elemento para trabalhar com horário, podendo também determinar mínimo e máximo de data. Campo de calendário visual será automático. 
    
    `<input type="datetime-local">` Elemento com as duas tags acima dentro do mesmo componente. 
    
    `<input type="month">` Meses da data selecionada.
    
    `<input type="week">` Semanas da data selecionada.
    
    `<input type="hidden">` É um atributo booleano que indica se um elemento é ou não relevante. Por exemplo, ele pode ser usado para esconder elementos de página que não podem ser usados até que o processo de login seja completo. Não é um elemento visível que passa informações/valores de gravação de dados.
    
    `<input type="color">` Permite que o usuário selecione uma cor(Podendo ser utilizado para templates com Javascript para personalização de preferência do usuário para uma melhor experiência).
    
    `<input type="email">` Possui autovalidação de e-mail, ou seja, com obrigatóriedade de completar o campo com uma informação válida. 
    
    `<input type="image">` Permite a inserção de uma imagem para o formulário, substituindo o botão de enviar. 
    
    `<input type="tel">` Precisa de propriedade `pattern` e `placeholder` para indicar um padrão de número de telefone: 
    * `pattern="\([0-9]{2}\)"` sendo `\( \)` Especificando *( )* parenteses e `[0-9]{2}` dois digitos de 0 à 9.
    * `pattern="\([0-9]{2}\)[9]{1}"` sendo `[9]{1}` dando obrigatoriedade iniciar com digito 9.
    * `pattern="\([0-9]{2}\)[9]{1}"[0-9]{4}` sendo `[0-9]{4}` onde o usuário preencherá 4 digitos de 0 a 9.
    * `pattern="\([0-9]{2}\)[9]{1}"[0-9]{4}-` será printado "-"
    * `pattern="\([0-9]{2}\)[9]{1}"[0-9]{4}-[0-9]{4}` sendo `[0-9]{4}` onde o usuário preencherá os 4 últimos dígitos de 0 à 9.
    * (xx)9xxxx-xxxx 

    `<input type="number">` Permite selecionar números. 
    
    `<input type="number" name=f_numero step="2" min="0" max="10">` Sendo indicação `min="0"` que o mínimo é 0 e `max="x"` o número máximo que aparecerá para selecionar e `step="x"` indica quantos caracteres é permitido, nesse mesmo exemplo `step="2"` que será *xx* ou ainda `step="3"` *xxx* por preferência do programador.  
  
    `<input type="search">` Campo de texto próprio para entrada de string para pesquisa. Contém padrão pré-definido, podendo usar JavaScript e PHP em sua elaboração. 
    
    

    
    
    
    
* *input* não contém fechamento.

***
***
***

* Display:
* Categoria: 
* Atributos:
* Contém fechamento:

`<ins>` Representa uma inserção/ algo que foi inserigo ao texto original. Sublinhado.

`<ins cite="url" datetime="">Texto visível e sublinhado (inserido)</ins>`

Quando aplicado o atributo `<cite>` é para direcionar a url com o motivo que o conteúdo foi inserido.
Quando aplicado o atributo `<datetime>` é para instruir o usuário a data e hora que esse conteúdo foi inserido.

* Display: Inline-block
* Categorria: Fluxo, contido por fraseado
* Atributos: Cite; Datetime; Globais
* Contém fechamento `</ins>`

***

`<pre>` Apresenta um bloco de texto pré formatado. 

* Display: Block
* Categoria: Fluxo
* Atributo: Globais; code; cols; width; wrap;
* Contém fechamento `</pre>`

***
***

> :construction: Esse documento está em construção 
> 
> :construction: Fernanda Evangelista 
> 
> :construction: Última atualização 13/04/2022 
