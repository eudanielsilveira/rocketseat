# Cascading Stylesheet

## O que é CSS  

- Folha de estilo em cascata
- Propriedade e valor
- Estilos para o HTML
- Arquivos `.css`

CSS, ou Cascading Style Sheet, é fundamental para dar estilo ao HTML, permitindo empilhar estilos em um arquivo .css. A regra de cascata possibilita modificar a página ao adicionar propriedades e valores, como cores e posicionamentos.

## Comentários

Comentários em CSS são úteis para fazer anotações e desconsiderar partes do código. Eles são criados com /* texto */, permitindo adicionar notas ou desativar trechos de código. Comentários ajudam a organizar e documentar o CSS de forma eficiente.

```css
/*
    Comentários
*/
```

## Anatomia

```css
/*
    Anatomia
    * Declaration
    * Selector
    * {} - context
    * Properties
    * Property value
*/
h1 {
    color: blue;
    font-size: 60px;
    letter-spacing: 2;
    text-transform: uppercase;
}
```
## Cascading

A hierarquia de regras aplicadas no CSS é fundamental. A cascata segue a ordem em que as regras são definidas, priorizando a última regra inserida. Mesmo com avisos de repetição, em documentos extensos, a última regra definida é a que prevalece. A ideia é que o último elemento na hierarquia de regras seja considerado. Isso é importante para entender como as cores e estilos são aplicados em diferentes elementos.

```css
/*
    Cascading
    - Cascata
    - Hierarquia de regras
*/
p {
    color: violet;
}

.green {
    color: green;
}
```
# Valores e unidades de medidas

Cada propriedade possui valores
`property: value`

```css
h1 {
    color: blue; /* color */
    font-size: 32px; /* length */
    letter-spacing: 2; /* number */
    text-transform: uppercase; /* ? */
}
```
`<data-type>`
> Estudo constante a fim de entender as propriedades e seus valores
>
> # Seletores
>```css
/*
    - type | element | tag
    -id = #
    - class = .nome
    - atributo = [nome]
    - universal = *
*/
p {
    color: violet;
}
>```
## Seletor de atributo

```html
<p  title> Lorem </>
```
```css
[title] {
    color: blue; /* color */
    font-size: 32px; /* length */
    letter-spacing: 2; /* number */
    text-transform: uppercase; /* ? */
}
```
# Propriedades para imagens
## object-position  

A propriedade CSS object-position especifica o alinhamento do conteúdo do elemento substituído selecionado dentro da caixa do elemento. As áreas da caixa que não são cobertas pelo objeto do elemento substituído mostrarão o fundo do elemento.  

```css

.element_one {
    object-position: 50% 50%;
}

.element_two {
    object-position: right top;
}

.element_three {
    object-position: left bottom;
}

.element_four {
    object-position: 250px 125px;
}
```
## object-fit

A propriedade CSS object-fit define como o conteúdo de um elemento substituído, como <img> ou <video>, deve ser redimensionado para caber em seu contêiner.  
```css

.element_one {
    object-fit: fill;
}

.element_two {
    object-fit: contain;
}

.element_three {
    object-fit: cover;
}

.element_four {
    object-fit: none;
}

.element_five {
    object-fit: scale-down;
}
```
