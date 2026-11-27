---
title: "ListBoxActiveXControl.ShowColumnHeads"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl egenskap. Anger om kolumnrubriker visas"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/showcolumnheads/
---
## ListBoxActiveXControl.ShowColumnHeads property

Anger om kolumnrubriker visas.

```csharp
public bool ShowColumnHeads { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyShowColumnHeadsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ListBox ActiveX‑kontroll med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ListBox, 
                1, 1, 100, 100,  // Left, Top, Width, Height
                0, 0);           // UpperLeftRow, UpperLeftColumn

            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper för ListBoxen
            listBox.ColumnCount = 2;
            listBox.ListWidth = 150;
            listBox.ShowColumnHeads = true; // Demonstrate ShowColumnHeads property

            // Lägg till lite exempeldata
            listBox.Value = "Header1\tHeader2\nItem1\tData1\nItem2\tData2";

            // Spara arbetsboken
            workbook.Save("ListBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


