---
title: "ListBox.ItemCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBox-egenskap. Hämtar antalet objekt i listboxen"
type: docs
url: /sv/net/aspose.cells.drawing/listbox/itemcount/
---
## ListBox.ItemCount property

Hämtar antalet objekt i listboxen.

```csharp
public int ItemCount { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyItemCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("Sheet1");

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Mango");

            // Skapa listbox och ställ in egenskaperna
            Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 10, 0, 100, 150);
            listBox.InputRange = "A1:A4";
            
            // Visa hur ItemCount används
            int itemCount = listBox.ItemCount;
            Console.WriteLine("ListBox contains {0} items", itemCount);
            
            // Justera listboxens höjd baserat på antalet objekt
            listBox.Height = itemCount * 15;

            workbook.Save("ListBoxItemCountDemo.xlsx");
        }
    }
}
```

### Se även

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


