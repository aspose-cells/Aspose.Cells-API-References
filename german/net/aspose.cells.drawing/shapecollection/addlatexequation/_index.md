---
title: "ShapeCollection.AddLaTeXEquation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt dem Arbeitsblatt ein Gleichungsobjekt mit LaTeX-Formatzeichenfolgen hinzu."
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addlatexequation/
---
## ShapeCollection.AddLaTeXEquation method

Fügt ein Gleichungsobjekt zum Arbeitsblatt hinzu, das LaTeX-Formatzeichenketten verwendet.

```csharp
public TextBox AddLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, 
    int width, string latex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Der Index der obersten Zeile. |
| oben | Int32 | Der vertikale Versatz seiner oberen Zeile, in Pixeln. |
| leftColumn | Int32 | Der Index der linken Spalte. |
| links | Int32 | Der horizontale Versatz von seiner linken Spalte, in Pixeln. |
| Höhe | Int32 | Die Höhe der Gleichung, in Pixeln. |
| Breite | Int32 | Die Breite der Gleichung, in Pixeln. |
| latex | String | LaTeX-Formatzeichenkette |

### Beispiele

```csharp

[C#]
// LaTeX-Formatzeichenkette.
string latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
// Fügt ein Gleichungsobjekt zum Arbeitsblatt hinzu.
TextBox textBox = shapes.AddLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

### Siehe auch

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


