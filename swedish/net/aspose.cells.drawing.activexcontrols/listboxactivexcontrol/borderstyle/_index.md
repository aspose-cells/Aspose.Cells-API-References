---
title: "ListBoxActiveXControl.BorderStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl egenskap. Hämtar och anger typen av ram som används av kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/borderstyle/
---
## ListBoxActiveXControl.BorderStyle property

Hämtar och anger typen av ram som används av kontrollen.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ListBox ActiveX‑kontroll med korrigerade parametrar
            Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 
                1, 0, 1, 100, 150, 30); // Added height parameter
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Ange BorderStyle‑egenskap
            listBox.BorderStyle = ControlBorderType.None;

            // Verifiera och skriv ut ramstil
            Console.WriteLine("BorderStyle: " + listBox.BorderStyle);

            workbook.Save("ListBoxBorderStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlBorderType](../../controlbordertype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


