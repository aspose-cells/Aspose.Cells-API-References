---
title: "ListBoxActiveXControl.SelectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl egenskap. Anger om kontrollen tillåter flera markeringar"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/selectiontype/
---
## ListBoxActiveXControl.SelectionType property

Anger om kontrollen tillåter flera val.

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
    public class ListBoxActiveXControlPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Lägg till ListBox ActiveX‑kontroll
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Konfigurera ListBox‑egenskaper
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            
            // Demonstrera SelectionType-egenskapen
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.Value = "Apple;Banana;Cherry";

            // Spara arbetsboken
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");

            Console.WriteLine("ListBox with Single SelectionType created successfully.");
        }
    }
}
```

### Se även

* enum [SelectionType](../../../aspose.cells.drawing/selectiontype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


