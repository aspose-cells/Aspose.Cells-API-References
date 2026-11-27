---
title: "SpinButtonActiveXControl.Max"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpinButtonActiveXControl-egenskap. Hämtar och anger det maximalt accepterade värdet"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max/
---
## SpinButtonActiveXControl.Max property

Hämtar och anger det maximalt accepterade värdet.

```csharp
public int Max { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMaxDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en SpinButton ActiveX-kontroll till kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 1, 1, 1, 100, 30);
            
            // Hämta ActiveX‑kontrollen och ange dess Max‑egenskap
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Max = 100;
            
            // Spara arbetsboken
            workbook.Save("SpinButtonMaxDemo.xlsx");
        }
    }
}
```

### Se även

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


