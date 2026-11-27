---
title: "LabelActiveXControl.SpecialEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LabelActiveXControl egenskap. Hämtar och anger den speciella effekten för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/specialeffect/
---
## LabelActiveXControl.SpecialEffect property

Hämtar och anger den speciella effekten för kontrollen.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en Label ActiveX Control med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 100, 50,  // upperLeftRow, upperLeftColumn, height, width
                100, 50);       // heightInPx, widthInPx
            LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;

            // Ställ in grundläggande egenskaper
            labelControl.Caption = "Sample Label";
            labelControl.IsWordWrapped = true;

            // Demonstrera egenskapen SpecialEffect
            labelControl.SpecialEffect = ControlSpecialEffectType.Raised;
            Console.WriteLine("SpecialEffect set to: " + labelControl.SpecialEffect);

            // Ändra SpecialEffect och visa skillnaden
            labelControl.SpecialEffect = ControlSpecialEffectType.Sunken;
            Console.WriteLine("SpecialEffect changed to: " + labelControl.SpecialEffect);

            // Spara arbetsboken
            workbook.Save("LabelActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


