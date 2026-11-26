---
title: "ShapeCollection.AddLaTeXEquation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega un objeto de ecuación a la hoja de cálculo usando cadenas de formato LaTeX"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addlatexequation/
---
## ShapeCollection.AddLaTeXEquation method

Agrega un objeto de ecuación a la hoja de cálculo usando cadenas con formato LaTeX.

```csharp
public TextBox AddLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, 
    int width, string latex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | El índice de la fila superior. |
| superior | Int32 | El desplazamiento vertical de su fila superior, en unidades de píxel. |
| leftColumn | Int32 | El índice de la columna izquierda. |
| izquierda | Int32 | El desplazamiento horizontal desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | La altura de la ecuación, en unidades de píxel. |
| ancho | Int32 | El ancho de la ecuación, en unidades de píxel. |
| latex | String | Cadena de formato LaTeX |

### Ejemplos

```csharp

[C#]
// Cadena de formato LaTeX.
string latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
// Agrega un objeto de ecuación a la hoja de cálculo.
TextBox textBox = shapes.AddLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

### Ver también

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


