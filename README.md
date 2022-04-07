# HTML5
Documento sobre a linguagem de marcação de construção de páginas 
Linguagem de Marcação de HiperTexto - Independente do editor de texto utilizado essa linguagem de marcação poderá ser utilizada na construção de páginas de web. 

Validate de estrutura [W3C](https://validator.w3.org/)

## 

 `<!DOCTYPE html>`é a instrução para o browser(navegador) de qual versão do HTML estamos trabalhando.

Os comandos de HTML são utilizados dentro de tags. As tags contém comandos, parâmetros e valores dos parâmetros.

##
```
<html lang="pt-BR">
</html>
```

O `<html` é a tag container raiz/root para todo o contéudo que será trabalhado no projeto. `lang=" "` é o parâmetro que vai indicar a linguagem de todo o projeto, e o que fica dentro de `" "` é o valor desse parâmetro, no caso o idioma português do Brasil `pt-BR` contém símbolos e caracteres que em outras linguagens não são utilizadas, então ao colocar esse valor no parâmetro indicamos que esse projeto irá conter todos os caracteres desse idioma e possibilitará que seja lido pelo browser. 

* Contém fechamento `</html>` 

##

`<head>` Cabeça da página - É o container para outras tags exclusivas que não são visíveis e sim de definições e configurações. 

* Filho de `<html>`
* Contém fechamento `</head>` 

##

`<title>` filha de `<head>` que representa o título da página que é mostrado na barra de título no browser. 

* Filho de `<head>`
* Contém fechamento `</title>`

##

`<body>` Tag Corpo da página. É o container de todos os elementos vísivel da página.

* Filho de `<html>`
* Contém fechamento `</body>`  

##

`<p>` Tag de parágrafo e possui pré configurações. 
* Elemento de fluxo - Elemento que marca o contéudo no corpo da página (visual).  
* Display Block - significa que não aceita um contéudo na mesma linha que ele, automaticamente quebra linha.
* Filho de `<body>`
* Contém fechamento `</p>`

##

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

##






 
