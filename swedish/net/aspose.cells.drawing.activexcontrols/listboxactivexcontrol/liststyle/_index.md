---
title: "ListBoxActiveXControl.ListStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl-egenskap. Hämtar och anger det visuella utseendet"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/liststyle/
---
## ListBoxActiveXControl.ListStyle property

Hämtar och anger det visuella utseendet.

```csharp
public ControlListStyle ListStyle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyListStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för listboxen
            sheet.Cells["A3"].Value = "Sales";
            sheet.Cells["A4"].Value = "Finance";
            sheet.Cells["A5"].Value = "MIS";
            sheet.Cells["A6"].Value = "R&D";
            sheet.Cells["A7"].Value = "Marketing";

            // Lägg till en ListBox ActiveX-kontroll
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Konfigurera ListBox-egenskaperna
            listBox.ListFillRange = "A3:A7";
            listBox.LinkedCell = "B1";
            listBox.ListStyle = ControlListStyle.Option; // Demonstrating ListStyle property
            listBox.SelectionType = SelectionType.Single;

            // Spara arbetsboken
            workbook.Save("ListBoxActiveXControl_ListStyle_Demo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlListStyle](../../controlliststyle/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


