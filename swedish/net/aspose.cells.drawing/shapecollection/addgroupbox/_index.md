---
title: "ShapeCollection.AddGroupBox"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en GroupBox i arbetsbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addgroupbox/
---
## ShapeCollection.AddGroupBox method

Lägger till en GroupBox i kalkylbladet.

```csharp
public GroupBox AddGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar den vertikala förskjutningen av GroupBox från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar den horisontella förskjutningen av GroupBox från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Representerar höjden på GroupBox, i enhet pixel. |
| bredd | Int32 | Representerar bredden på GroupBox, i enhet pixel. |

### Returvärde

Ett GroupBox-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddGroupBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en GroupBox i arbetsbladet
            ShapeCollection shapes = worksheet.Shapes;
            Aspose.Cells.Drawing.GroupBox groupBox = shapes.AddGroupBox(1, 0, 1, 0, 100, 50);

            // Spara arbetsboken
            workbook.Save("GroupBoxDemo.xlsx");
        }
    }
}
```

### Se även

* class [GroupBox](../../groupbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


