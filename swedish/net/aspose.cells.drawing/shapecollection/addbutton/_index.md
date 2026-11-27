---
title: "ShapeCollection.AddButton"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en Button till kalkylbladet."
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addbutton/
---
## ShapeCollection.AddButton method

Lägger till en Button i kalkylbladet.

```csharp
public Button AddButton(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala offsetet för Button från dess vänstra rad, i enheten pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar det horisontella offsetet för Button från dess vänstra kolumn, i enheten pixel. |
| höjd | Int32 | Representerar höjden på Button, i enheten pixel. |
| bredd | Int32 | Representerar bredden på Button, i enheten pixel. |

### Returvärde

Ett Button-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en knapp med de angivna parametrarna
            Aspose.Cells.Drawing.Button button = worksheet.Shapes.AddButton(1, 0, 1, 0, 100, 50);
            button.Text = "Click Me";

            // Spara arbetsboken
            workbook.Save("ButtonDemo.xlsx");
        }
    }
}
```

### Se även

* class [Button](../../button/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


