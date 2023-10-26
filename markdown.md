## Cabeçalho - Header
# Nível 1
## Nível 2
### Nível 3
#### Nível 4
##### Nível 5
###### Nível 6

```markdown
# Nível 1
## Nível 2
### Nível 3
#### Nível 4
##### Nível 5
###### Nível 6
```

## Negrito - Bold
**Texto em negrito** ou __Texto em negrito__
```markdown
**This is bold**, and so is __this__.
```
  
## Itálico - Italic
*Texto em itálico* ou _Texto em itálico_
```markdown
*Texto em itálico* ou _Texto em itálico_
```

## Tachado - Strike
~~Texto tachado~~, ou ~texto tachado~.
```markdown
~~Texto tachado~~, ou ~texto tachado~.
```

## Combinado (Negrito / Itálico) - Combine (Bold / Italic)
Combinado **_negrito com itálico_** é suportado
```markdown
Combinado **_negrito com itálico_** é suportado
```

## Caixa de marcação - CheckBox
- [ ] Desmarcada
- [X] Marcada
```markdown
- [ ] Desmacada
- [X] Desmacada
```

## Link e URLs
URL direta: https://github.com/JTheiller/sintax/edit/main/markdown.md
```markdown
URL direta: https://github.com/JTheiller/sintax/edit/main/markdown.md
```
Texto com URL: [JTheiller sintax Markdown](https://github.com/JTheiller/sintax/edit/main/markdown.md)
```markdown
Texto com URL: [JTheiller sintax Markdown](https://github.com/JTheiller/sintax/edit/main/markdown.md)
```

## Cor - Color
<font color="red">Texto com cor vermelha</font>
```markdown
<font color=\"red\">Texto com cor vermelha</font>
```

## Código - Code
Texto com `código`
````
Texto com `código`
````

## Bloco de código - Code blocks
```
Bloco de código - Code blocks
```
````
```
Bloco de código - Code blocks
Bloco de código - Code blocks
Bloco de código - Code blocks
```
````

## Realce de sintaxe - Syntax highlighting
```pascal
procedure Somar;
var
  LocalVar: Integer;
begin
  //...
end;
```
````
```pascal
procedure Somar;
var
  LocalVar: Integer;
begin
  //...
end;
```
````

## Seções recolhidas - collapsed sections
<details>
<summary>Clique aqui para abrir a seção recolhida e ver os detalhes</summary>
  
## Header
  
You can add text within a collapsed section. 

You can add an image or a code block, too.

```ruby
   puts "Hello World"
```
</details>

````markdown
<details>
<summary>Clique aqui para abrir a seção recolhida e ver os detalhes</summary>
  
### Header
  
You can add text within a collapsed section. 

You can add an image or a code block, too.

```ruby
   puts "Hello World"
```
</details>
````

## Tabelas - Tables
| Código | Descricao | Total |
| :--- | :---: | ---: |
| 1 | Minhas descricao | 0|
| 2 | Outras descrição `muito longa` para **analisar** alinhamento | 10 |
| A | Teste | 1000 |
```markdown
| Código | Descricao | Total |
| :--- | :---: | ---: |
| 1 | Minhas descricao | 0|
| 2 | Outras descrição `muito longa` para **analisar** alinhamento | 10 |
| A | Teste | 1000 |
```

## Destaque - Highlight
==Texto em destaque==
```markdown
==Texto em destaque==
```

## Expressões matemáticas - Mathematical expressions
- Utilize a senteça com delimitadores: `$[expressão]$`, ou bloco `math`.
- Utiliza o simpolo `\` para especificar as formulas.

$\sqrt{3x-1}+(1+x)^2$
```
$\sqrt{3x-1}+(1+x)^2$
```
$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$
````
```math
\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
```
````
