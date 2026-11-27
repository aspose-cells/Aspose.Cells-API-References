---
title: "ShapeCollection.AddLabel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en etikett i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addlabel/
---
## ShapeCollection.AddLabel method

Lägger till en Label i kalkylbladet.

```csharp
public Label AddLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar den vertikala förskjutningen av Label från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar den horisontella förskjutningen av Label från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Representerar höjden på Label, i enhet pixel. |
| bredd | Int32 | Representerar bredden på Label, i enhet pixel. |

### Returvärde

Ett Label-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLabelWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av former
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till en etikett i kalkylbladet
            Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
            label.Text = "Sample Label";

            // Spara arbetsboken
            workbook.Save("AddLabelDemo.xlsx");
        }
    }
}
```

### Se även

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


