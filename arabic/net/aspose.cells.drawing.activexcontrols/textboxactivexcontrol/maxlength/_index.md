---
title: "TextBoxActiveXControl.MaxLength"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxActiveXControl. تحصل وتضبط الحد الأقصى لعدد الأحرف"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/maxlength/
---
## TextBoxActiveXControl.MaxLength property

يحصل على الحد الأقصى لعدد الأحرف ويضبطه

```csharp
public int MaxLength { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyMaxLengthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم TextBox ActiveX والحصول على خاصية ActiveXControl الخاصة به
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // تعيين خاصية MaxLength
            if (textBox.MaxLength == 0)
            {
                textBox.MaxLength = 30;
            }

            // احفظ المصنف
            workbook.Save("TextBoxMaxLengthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


