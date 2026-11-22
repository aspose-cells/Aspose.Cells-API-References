---
title: "TextBoxActiveXControl.Text"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxActiveXControl. تسترجع وتضبط نص العنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/text/
---
## TextBoxActiveXControl.Text property

يحصل ويضبط نص العنصر.

```csharp
public string Text { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة عنصر تحكم ActiveX TextBox إلى ورقة العمل
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            
            // احصل على عنصر التحكم ActiveX وضع نصه
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
            textBox.Text = "This is a test.";
            
            // احفظ المصنف
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


