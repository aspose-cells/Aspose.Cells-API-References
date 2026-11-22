---
title: "TextBoxActiveXControl.PasswordChar"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxActiveXControl. تحصل وتضبط حرفًا يُعرض بدلاً من الأحرف المدخلة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/passwordchar/
---
## TextBoxActiveXControl.PasswordChar property

يحصل ويضبط حرفًا يتم عرضه بدلاً من الأحرف المدخلة.

```csharp
public char PasswordChar { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyPasswordCharDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم TextBox ActiveX والحصول على شكله
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 0, 1, 1, 100, 50);
            
            // الحصول على TextBoxActiveXControl من الشكل
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBoxControl = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // تعيين خاصية PasswordChar
            textBoxControl.PasswordChar = '*';

            // تعيين بعض النص لتوضيح إخفاء كلمة المرور
            textBoxControl.Text = "password123";

            // احفظ المصنف
            workbook.Save("TextBoxActiveXControlPasswordCharDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


