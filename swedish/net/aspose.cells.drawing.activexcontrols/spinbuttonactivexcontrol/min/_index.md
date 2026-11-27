---
title: "SpinButtonActiveXControl.Min"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpinButtonActiveXControl-egenskap. Hämtar och anger det minsta accepterade värdet"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min/
---
## SpinButtonActiveXControl.Min property

Hämtar och anger det minimalt accepterade värdet.

```csharp
public int Min { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMinDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en SpinButton ActiveX-kontroll till kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            
            // Ange Min-egenskapen för SpinButton
            spinButton.Min = 0;
            
            // Ange andra egenskaper för att demonstrera funktionaliteten
            spinButton.Max = 100;
            spinButton.Position = 50;
            
            // Spara arbetsboken
            workbook.Save("SpinButtonMinDemo.xlsx");
        }
    }
}
```

### Se även

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


