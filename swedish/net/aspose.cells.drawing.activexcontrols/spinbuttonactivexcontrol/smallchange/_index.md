---
title: "SpinButtonActiveXControl.SmallChange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpinButtonActiveXControl-egenskap. Hämtar och anger mängden som Position‑egenskapen ändras med"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/smallchange/
---
## SpinButtonActiveXControl.SmallChange property

Hämtar och anger mängden som Position-egenskapen ändras med

```csharp
public int SmallChange { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertySmallChangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en SpinButton ActiveX-kontroll till kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
            
            // Hämta ActiveX‑kontrollen och ange SmallChange‑egenskapen
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.SmallChange = 5;
            
            // Spara arbetsboken
            workbook.Save("SpinButtonSmallChangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


