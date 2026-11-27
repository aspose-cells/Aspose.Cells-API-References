---
title: "ShapeCollection.AddOval"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en Oval i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addoval/
---
## ShapeCollection.AddOval method

Lägger till en oval i kalkylbladet.

```csharp
public Oval AddOval(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala offsetet för Oval från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar det horisontella offsetet för Oval från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Representerar höjden på Oval, i enhet pixel. |
| bredd | Int32 | Representerar bredden på Oval, i enhet pixel. |

### Returvärde

Ett Oval-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddOvalWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en oval form i kalkylbladet
            ShapeCollection shapes = worksheet.Shapes;
            Oval oval = shapes.AddOval(1, 0, 1, 0, 50, 50);

            // Spara arbetsboken
            workbook.Save("AddOvalDemo.xlsx");
        }
    }
}
```

### Se även

* class [Oval](../../oval/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


