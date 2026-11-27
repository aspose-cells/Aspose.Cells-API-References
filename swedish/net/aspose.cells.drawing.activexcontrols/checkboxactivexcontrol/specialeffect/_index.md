---
title: "CheckBoxActiveXControl.SpecialEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxActiveXControl-egenskap. Hämtar och anger den speciella effekten för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/specialeffect/
---
## CheckBoxActiveXControl.SpecialEffect property

Hämtar och anger den speciella effekten för kontrollen.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 5, 0, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.CheckBoxActiveXControl checkBox = (Aspose.Cells.Drawing.ActiveXControls.CheckBoxActiveXControl)shape.ActiveXControl;

            checkBox.Caption = "Sample CheckBox";
            checkBox.SpecialEffect = Aspose.Cells.Drawing.ActiveXControls.ControlSpecialEffectType.Raised;
            
            workbook.Save("CheckBoxSpecialEffectDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


