---
title: "SpinButtonActiveXControl.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpinButtonActiveXControl-egenskap. Hämtar typen av ActiveX‑kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type/
---
## SpinButtonActiveXControl.Type property

Hämtar typen av ActiveX-kontrollen.

```csharp
public override ControlType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en SpinButton ActiveX‑kontroll (parametrar: left, top, width, height)
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 30, 100, 30);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;
            
            // Kontrollera kontrolltypen med Type‑egenskapen
            if (spinButton.Type == ControlType.SpinButton)
            {
                // Ange några egenskaper som är specifika för SpinButton
                spinButton.Min = 0;
                spinButton.Max = 100;
                spinButton.Position = 50;
                spinButton.SmallChange = 1;
            }
            
            // Spara arbetsboken
            workbook.Save("SpinButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlType](../../controltype/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


