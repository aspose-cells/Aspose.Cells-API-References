---
title: "ListBox.ItemCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBox‑Eigenschaft. Gibt die Anzahl der Elemente in der ListBox zurück"
type: docs
url: /de/net/aspose.cells.drawing/listbox/itemcount/
---
## ListBox.ItemCount property

Ermittelt die Anzahl der Elemente im Listenfeld.

```csharp
public int ItemCount { get; }
```

### Beispiele

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

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Mango");

            // Erstelle ListBox und setze Eigenschaften
            Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 10, 0, 100, 150);
            listBox.InputRange = "A1:A4";
            
            // Demonstriere die Verwendung von ItemCount
            int itemCount = listBox.ItemCount;
            Console.WriteLine("ListBox contains {0} items", itemCount);
            
            // Passe die Höhe der ListBox basierend auf der Elementanzahl an
            listBox.Height = itemCount * 15;

            workbook.Save("ListBoxItemCountDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


