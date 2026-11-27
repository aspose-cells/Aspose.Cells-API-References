---
title: "ShapeCollection.AddTextBox"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection‑metod. Lägger till en textruta i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addtextbox/
---
## ShapeCollection.AddTextBox method

Lägger till en textruta i kalkylbladet.

```csharp
public TextBox AddTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar den vertikala förskjutningen för textrutan från dess översta rad, i pixelenheter. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar den horisontella förskjutningen för textrutan från dess vänstra kolumn, i pixelenheter. |
| höjd | Int32 | Representerar höjden på textrutan, i pixelenheter. |
| bredd | Int32 | Representerar bredden på textrutan, i pixelenheter. |

### Returvärde

Ett [`TextBox`](../../textbox/)‑objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av former
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till en TextBox med angiven position och storlek
            TextBox textBox = shapes.AddTextBox(1, 0, 1, 0, 100, 50);
            textBox.Text = "Sample TextBox";

            // Spara arbetsboken
            workbook.Save("TextBoxDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


