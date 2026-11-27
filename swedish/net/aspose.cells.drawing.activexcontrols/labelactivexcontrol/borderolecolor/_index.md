---
title: "LabelActiveXControl.BorderOleColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LabelActiveXControl-egenskap. Hämtar och ställer in ole-färgen för bakgrunden"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/borderolecolor/
---
## LabelActiveXControl.BorderOleColor property

Hämtar och anger ole-färgen för bakgrunden.

```csharp
public int BorderOleColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en Label ActiveX Control
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Label, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl labelControl = 
                (Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper
            labelControl.Caption = "Sample Label";
            labelControl.BorderOleColor = -2147483642; // Set border color (OLE_COLOR)
            labelControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            
            // Spara arbetsboken
            workbook.Save("LabelActiveXControlBorderOleColorDemo.xlsx");

            // Visa kantfärgen
            Console.WriteLine("BorderOleColor: " + labelControl.BorderOleColor);
        }
    }
}
```

### Se även

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


