---
title: "ListBoxActiveXControl.ListWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl egenskap. Hämtar och sätter bredden i enheter av punkter"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/listwidth/
---
## ListBoxActiveXControl.ListWidth property

Hämtar och anger bredden i enheter av punkter.

```csharp
public double ListWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyListWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ListBox ActiveX-kontroll med alla nödvändiga parametrar
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 
                10, 10, 200, 100, 200, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Ställ in ListWidth-egenskapen
            listBox.ListWidth = 150;
            
            // Konfigurera grundläggande egenskaper
            listBox.ColumnCount = 2;
            listBox.ColumnWidths = 100; // Changed from string to double
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Red");
            worksheet.Cells["B2"].PutValue("Yellow");
            worksheet.Cells["B3"].PutValue("Orange");
            
            // Ange dataområde
            listBox.ListFillRange = "A1:B3";

            workbook.Save("ListBoxWidthDemo.xlsx");
            Console.WriteLine("ListBox with ListWidth=150 created successfully.");
        }
    }
}
```

### Se även

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


