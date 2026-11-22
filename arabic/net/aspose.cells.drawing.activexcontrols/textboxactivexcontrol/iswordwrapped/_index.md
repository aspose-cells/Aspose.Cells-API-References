---
title: "TextBoxActiveXControl.IsWordWrapped"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxActiveXControl. تشير إلى ما إذا كان محتوى التحكم يلتف تلقائيًا في نهاية السطر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iswordwrapped/
---
## TextBoxActiveXControl.IsWordWrapped property

يشير إلى ما إذا كان محتوى العنصر يلتف تلقائيًا في نهاية السطر.

```csharp
public bool IsWordWrapped { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم TextBox ActiveX مع جميع المعلمات المطلوبة
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox,
                1, 1, 200, 100, 0, 0);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // قم بتعيين بعض النص الذي سيستفيد من التفاف الكلمات
            textBox.Text = "This is a long text that should demonstrate word wrapping functionality in the TextBox ActiveX control.";

            // تحقق واضبط خاصية IsWordWrapped
            if (!textBox.IsWordWrapped)
            {
                textBox.IsWordWrapped = true;
                Console.WriteLine("Word wrapping has been enabled for the TextBox.");
            }

            // احفظ المصنف
            workbook.Save("TextBoxWordWrapDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


