---
title: "RadioButtonActiveXControl.Alignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RadioButtonActiveXControl egenskap. Hämtar och anger positionen för rubriken i förhållande till kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/alignment/
---
## RadioButtonActiveXControl.Alignment property

Hämtar och anger positionen för Caption relativt kontrollen.

```csharp
public ControlCaptionAlignmentType Alignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyAlignmentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en ny formsamling och lägg till ActiveX-kontroll
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.RadioButton, 1, 1, 100, 30, 0, 0);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;
            
            // Ställ in Alignment-egenskapen
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            
            // Spara arbetsboken
            workbook.Save("RadioButtonAlignmentDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


