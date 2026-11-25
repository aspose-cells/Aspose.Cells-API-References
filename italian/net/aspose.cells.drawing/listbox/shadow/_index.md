---
title: "ListBox.Shadow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBox. Indica se la combobox ha ombreggiatura 3D"
type: docs
url: /it/net/aspose.cells.drawing/listbox/shadow/
---
## ListBox.Shadow property

Indica se la combobox ha ombreggiatura 3D.

```csharp
public bool Shadow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola gli elementi della lista
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // Crea listbox e imposta le proprietà principali
            ListBox listBox = worksheet.Shapes.AddListBox(2, 1, 5, 1, 100, 150);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            // Imposta la proprietà shadow
            listBox.Shadow = true;

            // Salva e ricarica per verificare
            workbook.Save("ListBoxShadowDemo.xlsx");
            
            Workbook loadedWorkbook = new Workbook("ListBoxShadowDemo.xlsx");
            ListBox loadedBox = (ListBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            Console.WriteLine("Shadow enabled: " + loadedBox.Shadow);
        }
    }
}
```

### Vedi anche

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


