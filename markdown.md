O Markdown é uma linguagem de marcação simples, mas poderosa, amplamente utilizada para formatação de texto em ambientes digitais. Neste guia, iremos desvendar a sintaxe do Markdown, explorando os principais elementos que a compõem. Aprenderemos desde as noções básicas, como a formatação de texto, cabeçalhos e listas, até técnicas mais avançadas, como a inclusão de links, imagens e tabelas. Ao final desta exploração, você estará equipado com um sólido entendimento da estrutura e gramática do Markdown, permitindo que você crie documentos bem formatados de maneira eficiente em diversas plataformas online. Vamos começar a desvendar os segredos da sintaxe do Markdown e aproveitar ao máximo essa ferramenta versátil de formatação de texto.

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

## Subscript
H<sub>2</sub>O
```markdown
H<sub>2</sub>O
```

## Superscript
X<sup>2</sup>
```markdown
X<sup>2</sup>
```

## Tarefas - Task lists
- [ ] Desmarcada
- [X] Marcada
```markdown
- [ ] Desmarcada
- [X] Marcada
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

## Alertas - Alerts
> [!NOTE]
> Highlights information that users should take into account, even when skimming.

> [!IMPORTANT]
> Crucial information necessary for users to succeed.

> [!WARNING]
> Critical content demanding immediate user attention due to potential risks.
```markdown
> [!NOTE]
> Highlights information that users should take into account, even when skimming.

> [!IMPORTANT]
> Crucial information necessary for users to succeed.

> [!WARNING]
> Critical content demanding immediate user attention due to potential risks.
```

## Comentário oculto - Hiding content with comments
<!-- Esse comentário não será renderizado no Markdown -->
Esse trexo possui um comentário oculto
```markdown
<!-- Esse comentário não será renderizado no Markdown -->
Esse trexo possui um comentário oculto
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

## Diagramas de sereia - Mermaid diagrams

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

````
```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
````

## GeoJSON
```geojson
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "id": 1,
      "properties": {
        "ID": 0
      },
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
              [-90,35],
              [-90,30],
              [-85,30],
              [-85,35],
              [-90,35]
          ]
        ]
      }
    }
  ]
}
```

````markdown
```geojson
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "id": 1,
      "properties": {
        "ID": 0
      },
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
              [-90,35],
              [-90,30],
              [-85,30],
              [-85,35],
              [-90,35]
          ]
        ]
      }
    }
  ]
}
```
````

## TopoJSON
```topojson
{
  "type": "Topology",
  "transform": {
    "scale": [0.0005000500050005, 0.00010001000100010001],
    "translate": [100, 0]
  },
  "objects": {
    "example": {
      "type": "GeometryCollection",
      "geometries": [
        {
          "type": "Point",
          "properties": {"prop0": "value0"},
          "coordinates": [4000, 5000]
        },
        {
          "type": "LineString",
          "properties": {"prop0": "value0", "prop1": 0},
          "arcs": [0]
        },
        {
          "type": "Polygon",
          "properties": {"prop0": "value0",
            "prop1": {"this": "that"}
          },
          "arcs": [[1]]
        }
      ]
    }
  },
  "arcs": [[[4000, 0], [1999, 9999], [2000, -9999], [2000, 9999]],[[0, 0], [0, 9999], [2000, 0], [0, -9999], [-2000, 0]]]
}
```

````markdown
```topojson
{
  "type": "Topology",
  "transform": {
    "scale": [0.0005000500050005, 0.00010001000100010001],
    "translate": [100, 0]
  },
  "objects": {
    "example": {
      "type": "GeometryCollection",
      "geometries": [
        {
          "type": "Point",
          "properties": {"prop0": "value0"},
          "coordinates": [4000, 5000]
        },
        {
          "type": "LineString",
          "properties": {"prop0": "value0", "prop1": 0},
          "arcs": [0]
        },
        {
          "type": "Polygon",
          "properties": {"prop0": "value0",
            "prop1": {"this": "that"}
          },
          "arcs": [[1]]
        }
      ]
    }
  },
  "arcs": [[[4000, 0], [1999, 9999], [2000, -9999], [2000, 9999]],[[0, 0], [0, 9999], [2000, 0], [0, -9999], [-2000, 0]]]
}
```
````

## STL Modelo 3D - STL 3D models
```stl
solid cube_corner
  facet normal 0.0 -1.0 0.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 1.0 0.0 0.0
      vertex 0.0 0.0 1.0
    endloop
  endfacet
  facet normal 0.0 0.0 -1.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 0.0 1.0 0.0
      vertex 1.0 0.0 0.0
    endloop
  endfacet
  facet normal -1.0 0.0 0.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 0.0 0.0 1.0
      vertex 0.0 1.0 0.0
    endloop
  endfacet
  facet normal 0.577 0.577 0.577
    outer loop
      vertex 1.0 0.0 0.0
      vertex 0.0 1.0 0.0
      vertex 0.0 0.0 1.0
    endloop
  endfacet
endsolid
```

````markdown
```stl
solid cube_corner
  facet normal 0.0 -1.0 0.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 1.0 0.0 0.0
      vertex 0.0 0.0 1.0
    endloop
  endfacet
  facet normal 0.0 0.0 -1.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 0.0 1.0 0.0
      vertex 1.0 0.0 0.0
    endloop
  endfacet
  facet normal -1.0 0.0 0.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 0.0 0.0 1.0
      vertex 0.0 1.0 0.0
    endloop
  endfacet
  facet normal 0.577 0.577 0.577
    outer loop
      vertex 1.0 0.0 0.0
      vertex 0.0 1.0 0.0
      vertex 0.0 0.0 1.0
    endloop
  endfacet
endsolid
```
````

## Nota de rodapé - Footnote
Anotacao 1 - Existirá uma anotação simples apresentada no rodapé de todo texto o arquivo[^1].

Anotacao 2 - Existirá uma anotação com multiplas linhas apresentada no rodapé de todo texto o arquivo[^2].

[^1]: Anotação 1 - Referência.
[^2]: Anotações com multimas linhas, adicionado prefixo de duplo espaço.
  Esta é a segunda linha.
```markdown
Anotacao 1 - Existirá uma anotação simples apresentada no rodapé de todo texto o arquivo[^1].

Anotacao 2 - Existirá uma anotação com multiplas linhas apresentada no rodapé de todo texto o arquivo[^2].

[^1]: Anotação 1 - Referência.
[^2]: Anotações com multimas linhas, adicionado prefixo de duplo espaço.
  Esta é a segunda linha.
```
