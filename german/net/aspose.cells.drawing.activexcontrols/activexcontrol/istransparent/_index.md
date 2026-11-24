---
title: "ActiveXControl.IsTransparent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControl-Eigenschaft. Gibt an, ob das Steuerelement transparent ist"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/
---
## ActiveXControl.IsTransparent property

Gibt an, ob das Steuerelement transparent ist.

```csharp
public bool IsTransparent { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsTransparentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Form erstellen, um das ActiveX-Steuerelement mit allen erforderlichen Parametern zu hosten
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 200, 50, 
                0, 0); // Adding missing parameters for upperLeftRow, upperLeftColumn, height, width, left, top

            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Steuereigenschaften festlegen
            label.Caption = "Sample Label";
            label.IsTransparent = false; // Demonstrating IsTransparent property

            // Die IsTransparent-Eigenschaft überprüfen und ausgeben
            Console.WriteLine("Label IsTransparent property: " + label.IsTransparent);

            // Transparenz ändern und erneut überprüfen
            label.IsTransparent = true;
            Console.WriteLine("Label IsTransparent property after change: " + label.IsTransparent);

            // Speichere die Arbeitsmappe
            workbook.Save("ActiveXControlIsTransparentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


