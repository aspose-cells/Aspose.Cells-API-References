---
title: "TextBoxActiveXControl.SpecialEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl egenskap. Hämtar och anger den speciella effekten för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/specialeffect/
---
## TextBoxActiveXControl.SpecialEffect property

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
    public class TextBoxActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ActiveX TextBox-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 100, 100, 0, 0);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Ange SpecialEffect-egenskapen
            textBox.SpecialEffect = ControlSpecialEffectType.Bump;

            // Spara arbetsboken
            workbook.Save("TextBoxActiveXControlSpecialEffectDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


