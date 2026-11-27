---
title: "ListBox.SelectedIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBox-egenskap. Hämtar eller anger indexnumret för det för närvarande markerade objektet i en listbox eller kombinationsruta. Nollbaserad"
type: docs
url: /sv/net/aspose.cells.drawing/listbox/selectedindex/
---
## ListBox.SelectedIndex property

Hämtar eller anger indexnumret för det för närvarande markerade objektet i en listbox eller kombinationsruta. Nollbaserat.

```csharp
public int SelectedIndex { get; set; }
```

### Anmärkningar

-1 presents no item is selected.

### Exempel

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

### Se även

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


