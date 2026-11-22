---
title: "TextBoxActiveXControl.SpecialEffect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxActiveXControl. تسترجع وتضبط التأثير الخاص للعنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/specialeffect/
---
## TextBoxActiveXControl.SpecialEffect property

يحصل على التأثير الخاص للتحكم ويضبطه.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم TextBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 100, 100, 0, 0);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // اضبط خاصية SpecialEffect
            textBox.SpecialEffect = ControlSpecialEffectType.Bump;

            // احفظ المصنف
            workbook.Save("TextBoxActiveXControlSpecialEffectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


