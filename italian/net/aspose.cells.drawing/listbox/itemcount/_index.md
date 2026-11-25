---
title: "ListBox.ItemCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBox. Restituisce il numero di elementi nella casella di riepilogo"
type: docs
url: /it/net/aspose.cells.drawing/listbox/itemcount/
---
## ListBox.ItemCount property

Restituisce il numero di elementi nella casella di riepilogo.

```csharp
public int ItemCount { get; }
```

### Esempi

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

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Mango");

            // Crea una casella di riepilogo e imposta le proprietà
            Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 10, 0, 100, 150);
            listBox.InputRange = "A1:A4";
            
            // Dimostra l'uso di ItemCount
            int itemCount = listBox.ItemCount;
            Console.WriteLine("ListBox contains {0} items", itemCount);
            
            // Regola l'altezza della listbox in base al numero di elementi
            listBox.Height = itemCount * 15;

            workbook.Save("ListBoxItemCountDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


