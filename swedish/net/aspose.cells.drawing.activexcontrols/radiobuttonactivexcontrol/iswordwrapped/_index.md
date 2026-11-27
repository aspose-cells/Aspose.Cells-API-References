---
title: "RadioButtonActiveXControl.IsWordWrapped"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RadioButtonActiveXControl egenskap. Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/iswordwrapped/
---
## RadioButtonActiveXControl.IsWordWrapped property

Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad.

```csharp
public bool IsWordWrapped { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en RadioButton ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton,
                1, 1, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl radioButton = 
                (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape.ActiveXControl;

            // Demonstrera IsWordWrapped-egenskapen
            Console.WriteLine("Initial IsWordWrapped value: " + radioButton.IsWordWrapped);
            
            radioButton.IsWordWrapped = true;
            Console.WriteLine("After setting IsWordWrapped to true: " + radioButton.IsWordWrapped);
            
            radioButton.IsWordWrapped = false;
            Console.WriteLine("After setting IsWordWrapped to false: " + radioButton.IsWordWrapped);

            // Spara arbetsboken
            workbook.Save("RadioButtonIsWordWrappedDemo.xlsx");
        }
    }
}
```

### Se även

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


