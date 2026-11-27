---
title: "ListBoxActiveXControl.ColumnCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl egenskap. Representerar antalet kolumner som ska visas i en ComboBox eller ListBox"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/columncount/
---
## ListBoxActiveXControl.ColumnCount property

Representerar antalet kolumner som ska visas i en ComboBox eller ListBox.

```csharp
public int ColumnCount { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyColumnCountDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ListBox ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 1, 1, 1, 200, 100);
            var listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper inklusive ColumnCount
            listBox.ColumnCount = 3;
            listBox.ListFillRange = "A1:C3"; // Sample data range for 3 columns

            // Verifiera och skriv ut ColumnCount
            Console.WriteLine("ListBox ColumnCount: " + listBox.ColumnCount);

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


