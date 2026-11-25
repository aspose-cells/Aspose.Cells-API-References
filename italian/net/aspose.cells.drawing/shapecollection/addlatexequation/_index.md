---
title: "ShapeCollection.AddLaTeXEquation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un oggetto equazione al foglio di lavoro usando stringhe di formato LaTeX"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addlatexequation/
---
## ShapeCollection.AddLaTeXEquation method

Aggiunge un oggetto equazione al foglio di lavoro usando stringhe in formato LaTeX.

```csharp
public TextBox AddLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, 
    int width, string latex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | L'indice della riga superiore. |
| alto | Int32 | Lo scostamento verticale della sua riga superiore, in unità di pixel. |
| leftColumn | Int32 | L'indice della colonna sinistra. |
| sinistra | Int32 | Lo spostamento orizzontale dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | L'altezza dell'equazione, in unità di pixel. |
| larghezza | Int32 | La larghezza dell'equazione, in unità di pixel. |
| latex | String | Stringa di formato LaTeX |

### Esempi

```csharp

[C#]
// Stringa di formato LaTeX.
string latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
// Aggiunge un oggetto equazione al foglio di lavoro.
TextBox textBox = shapes.AddLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

### Vedi anche

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


