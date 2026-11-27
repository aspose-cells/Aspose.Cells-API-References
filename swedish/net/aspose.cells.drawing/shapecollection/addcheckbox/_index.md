---
title: "ShapeCollection.AddCheckBox"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en kryssruta i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addcheckbox/
---
## ShapeCollection.AddCheckBox method

Lägger till en kryssruta i kalkylbladet.

```csharp
public CheckBox AddCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar den vertikala förskjutningen av checkbox från dess översta rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar den horisontella förskjutningen för textrutan från dess vänstra kolumn, i pixelenheter. |
| höjd | Int32 | Höjd på textbox, i enhet pixel. |
| bredd | Int32 | Bredd på textbox, i enhet pixel. |

### Returvärde

Det nya CheckBox-objektets index.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCheckBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av former
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till en CheckBox med de angivna parametrarna
            Aspose.Cells.Drawing.CheckBox checkBox = shapes.AddCheckBox(1, 0, 1, 0, 100, 50);

            // Spara arbetsboken
            workbook.Save("CheckBoxDemo.xlsx");
        }
    }
}
```

### Se även

* class [CheckBox](../../checkbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


