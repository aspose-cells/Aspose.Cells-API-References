---
title: "TextBoxActiveXControl.IntegralHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxActiveXControl. تشير إلى ما إذا كان العنصر سيظهر فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/integralheight/
---
## TextBoxActiveXControl.IntegralHeight property

يُشير إلى ما إذا كان العنصر سيعرض فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية.

```csharp
public bool IntegralHeight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIntegralHeightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم ActiveX TextBox واحصل على خاصية ActiveXControl الخاصة به
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // اعرض خاصية IntegralHeight
            Console.WriteLine("Initial IntegralHeight: " + textBox.IntegralHeight);
            
            // اضبط IntegralHeight إلى true إذا كان false
            if (!textBox.IntegralHeight)
            {
                textBox.IntegralHeight = true;
                Console.WriteLine("IntegralHeight set to: " + textBox.IntegralHeight);
            }

            // احفظ المصنف
            workbook.Save("TextBoxActiveXControlIntegralHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


