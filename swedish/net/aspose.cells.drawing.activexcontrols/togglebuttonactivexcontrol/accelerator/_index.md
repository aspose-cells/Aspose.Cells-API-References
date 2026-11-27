---
title: "ToggleButtonActiveXControl.Accelerator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ToggleButtonActiveXControl-egenskap. Hämtar och anger acceleratortangenten för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator/
---
## ToggleButtonActiveXControl.Accelerator property

Hämtar och anger acceleratortangenten för kontrollen.

```csharp
public char Accelerator { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ToggleButton ActiveX-kontroll med korrekta parametrar
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 100, 30, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Ange egenskapen Accelerator
            toggleButton.Accelerator = 'A';
            Console.WriteLine("ToggleButton Accelerator set to: " + toggleButton.Accelerator);

            // Rensa egenskapen Accelerator
            toggleButton.Accelerator = '\0';
            Console.WriteLine("ToggleButton Accelerator cleared: " + (toggleButton.Accelerator == '\0' ? "True" : "False"));
        }
    }
}
```

### Se även

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


