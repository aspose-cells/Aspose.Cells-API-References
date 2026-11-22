---
title: "ActiveXControl.TextAlign"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControl. تمثل طريقة محاذاة النص المستخدم في العنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrol/textalign/
---
## ActiveXControl.TextAlign property

يمثل طريقة محاذاة النص المستخدم في العنصر.

```csharp
public TextAlignmentType TextAlign { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyTextAlignDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصرين checkbox ActiveX
            Shape shape1 = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 30);
            Shape shape2 = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 2, 0, 100, 30);

            // احصل على عناصر ActiveX
            CheckBoxActiveXControl checkbox1 = (CheckBoxActiveXControl)shape1.ActiveXControl;
            CheckBoxActiveXControl checkbox2 = (CheckBoxActiveXControl)shape2.ActiveXControl;

            // تعيين محاذاة نص مختلفة
            checkbox1.TextAlign = TextAlignmentType.Center;
            checkbox2.TextAlign = TextAlignmentType.Right;

            // عرض قيم محاذاة النص
            Console.WriteLine("Checkbox1 TextAlign: " + checkbox1.TextAlign);
            Console.WriteLine("Checkbox2 TextAlign: " + checkbox2.TextAlign);
        }
    }
}
```

### انظر أيضًا

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


