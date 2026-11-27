---
title: "ActiveXControlBase.Height"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControlBase-egenskap. Hämtar och anger kontrollens höjd i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/height/
---
## ActiveXControlBase.Height property

Hämtar och anger kontrollens höjd i enheter av punkter.

```csharp
public virtual double Height { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyHeightDemo
    {
        public static void Run()
        {
            // Initiera en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till en RadioButton ActiveXControl
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 50);
            RadioButtonActiveXControl activeXControl = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Ställ in grundläggande egenskaper
            activeXControl.Caption = "Height Demo";
            activeXControl.IsAutoSize = false; // Disable auto-size to demonstrate Height property

            // Demonstrera Height-egenskapen
            Console.WriteLine("Original Height: " + activeXControl.Height);
            activeXControl.Height = 75;
            Console.WriteLine("Modified Height: " + activeXControl.Height);

            // Spara arbetsboken
            workbook.Save("ActiveXControlHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


