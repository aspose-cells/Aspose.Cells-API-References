---
title: "CheckBoxActiveXControl.SpecialEffect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CheckBoxActiveXControl. تحصل وتضبط التأثير الخاص للعنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/specialeffect/
---
## CheckBoxActiveXControl.SpecialEffect property

يحصل على التأثير الخاص للتحكم ويضبطه.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### أمثلة

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

### انظر أيضًا

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


