---
title: "ShapeCollection.AddLaTeXEquation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till ett ekvationsobjekt i kalkylbladet med LaTeX-formatsträngar"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addlatexequation/
---
## ShapeCollection.AddLaTeXEquation method

Lägger till ett ekvationsobjekt i kalkylbladet med LaTeX-formatsträngar.

```csharp
public TextBox AddLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, 
    int width, string latex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Index för översta raden. |
| top | Int32 | Vertikal förskjutning för dess översta rad, i pixelenheter. |
| leftColumn | Int32 | Det vänstra kolumnindexet. |
| vänster | Int32 | Den horisontella förskjutningen från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Höjden på ekvationen, i enhet pixel. |
| bredd | Int32 | Bredden på ekvationen, i enhet pixel. |
| latex | String | LaTeX-formatsträng |

### Exempel

```csharp

[C#]
// LaTeX-formatsträng.
string latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
// Lägger till ett ekvationsobjekt i kalkylbladet.
TextBox textBox = shapes.AddLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

### Se även

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


