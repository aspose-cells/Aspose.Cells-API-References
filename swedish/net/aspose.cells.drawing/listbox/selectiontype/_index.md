---
title: "ListBox.SelectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBox-egenskap. Hämtar eller anger markeringsläget för den angivna listboxen"
type: docs
url: /sv/net/aspose.cells.drawing/listbox/selectiontype/
---
## ListBox.SelectionType property

Hämtar eller anger urvalsläget för den angivna listrutan.

```csharp
public SelectionType SelectionType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för listboxen
            sheet.Cells["A1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Finance");
            sheet.Cells["A3"].PutValue("MIS");
            sheet.Cells["A4"].PutValue("R&D");

            // Lägg till en listbox
            ListBox listBox = sheet.Shapes.AddListBox(1, 0, 2, 0, 100, 80);
            
            // Ställ in listboxegenskaper
            listBox.InputRange = "A1:A4";
            listBox.LinkedCell = "B1";
            
            // Demonstrera SelectionType-egenskapen
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.SelectedIndex = 1; // Select "Finance"

            // Spara arbetsboken
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SelectionType](../../selectiontype/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


