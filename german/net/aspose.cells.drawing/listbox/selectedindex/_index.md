---
title: "ListBox.SelectedIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBox-Eigenschaft. Gibt den Index des aktuell ausgewählten Elements in einer ListBox oder ComboBox zurück oder legt ihn fest. Nullbasiert"
type: docs
url: /de/net/aspose.cells.drawing/listbox/selectedindex/
---
## ListBox.SelectedIndex property

Ermittelt oder legt die Indexnummer des aktuell ausgewählten Elements in einem Listenfeld oder Kombinationsfeld fest. Nullbasiert.

```csharp
public int SelectedIndex { get; set; }
```

### Hinweise

-1 presents no item is selected.

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectedIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue("Item 0");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            
            ListBox listBox = worksheet.Shapes.AddListBox(5, 5, 100, 100, 200, 300);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            listBox.SelectedIndex = 2;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


