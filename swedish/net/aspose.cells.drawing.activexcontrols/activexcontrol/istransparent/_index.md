---
title: "ActiveXControl.IsTransparent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControl-egenskap. Anger om kontrollen är transparent"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/
---
## ActiveXControl.IsTransparent property

Anger om kontrollen är transparent.

```csharp
public bool IsTransparent { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form för att hysa ActiveX-kontrollen med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 200, 50, 
                0, 0); // Adding missing parameters for upperLeftRow, upperLeftColumn, height, width, left, top

            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Ställ in kontrollens egenskaper
            label.Caption = "Sample Label";
            label.IsTransparent = false; // Demonstrating IsTransparent property

            // Verifiera och skriv ut IsTransparent-egenskapen
            Console.WriteLine("Label IsTransparent property: " + label.IsTransparent);

            // Ändra transparens och verifiera igen
            label.IsTransparent = true;
            Console.WriteLine("Label IsTransparent property after change: " + label.IsTransparent);

            // Spara arbetsboken
            workbook.Save("ActiveXControlIsTransparentDemo.xlsx");
        }
    }
}
```

### Se även

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


