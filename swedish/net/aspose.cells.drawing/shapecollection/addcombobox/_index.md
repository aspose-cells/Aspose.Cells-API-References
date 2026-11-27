---
title: "ShapeCollection.AddComboBox"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en ComboBox i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addcombobox/
---
## ShapeCollection.AddComboBox method

Lägger till en ComboBox i kalkylbladet.

```csharp
public ComboBox AddComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar den vertikala förskjutningen av ComboBox från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar den horisontella förskjutningen av ComboBox från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Representerar höjden på ComboBox, i enhet pixel. |
| bredd | Int32 | Representerar bredden på ComboBox, i enhet pixel. |

### Returvärde

Ett ComboBox-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddComboBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av former
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till en kombinationsruta med angivna parametrar
            Aspose.Cells.Drawing.ComboBox comboBox = shapes.AddComboBox(1, 0, 1, 0, 100, 50);

            // Lägg till objekt i kombinationsrutan genom att ange cellvärden
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Ange inmatningsområdet för kombinationsrutan
            comboBox.InputRange = "A1:A3";
            comboBox.DropDownLines = 3;

            // Spara arbetsboken
            workbook.Save("AddComboBoxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ComboBox](../../combobox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


