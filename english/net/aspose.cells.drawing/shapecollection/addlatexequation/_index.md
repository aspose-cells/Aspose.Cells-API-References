---
title: ShapeCollection.AddLaTeXEquation
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds an equation object to the worksheet using LaTeX format strings
type: docs
url: /net/aspose.cells.drawing/shapecollection/addlatexequation/
---
## ShapeCollection.AddLaTeXEquation method

Adds an equation object to the worksheet using LaTeX format strings.

```csharp
public TextBox AddLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, 
    int width, string latex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | The top row index. |
| top | Int32 | The vertical offset its top row, in unit of pixel. |
| leftColumn | Int32 | The left column index. |
| left | Int32 | The horizontal offset from its left column, in unit of pixel. |
| height | Int32 | The height of equation, in unit of pixel. |
| width | Int32 | The width of equation, in unit of pixel. |
| latex | String | LaTeX format string |

### Examples

```csharp

[C#]
// LaTeX format string.
string latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
// Adds an equation object to the worksheet.
TextBox textBox = shapes.AddLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

### See Also

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


