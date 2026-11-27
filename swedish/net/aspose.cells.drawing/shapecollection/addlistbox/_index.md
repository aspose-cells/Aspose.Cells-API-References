---
title: "ShapeCollection.AddListBox"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en ListBox i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addlistbox/
---
## ShapeCollection.AddListBox method

Lägger till en ListBox i kalkylbladet.

```csharp
public ListBox AddListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala offsetet för ListBox från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar det horisontella offsetet för ListBox från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Representerar höjden på ListBox, i enhet pixel. |
| bredd | Int32 | Representerar bredden på ListBox, i enhet pixel. |

### Returvärde

Ett ListBox-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddListBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en listbox i kalkylbladet
            Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 50);

            // Lägg till objekt i listboxen
            listBox.SetInputRange("A1:A3", false, false);
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Spara arbetsboken
            workbook.Save("ListBoxDemo.xlsx");
        }
    }
}
```

### Se även

* class [ListBox](../../listbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


