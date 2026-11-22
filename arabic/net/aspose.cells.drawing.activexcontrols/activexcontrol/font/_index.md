---
title: "ActiveXControl.Font"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControl. تمثل خط العنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrol/font/
---
## ActiveXControl.Font property

يمثل خط العنصر.

```csharp
public Font Font { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlPropertyFontDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف عنصر ActiveX (Label) إلى ورقة العمل
                Shape shape = worksheet.Shapes.AddActiveXControl(
                    ControlType.Label,
                    1, 1, 200, 50,
                    0, 0);

                // احصل على مثيل عنصر ActiveX
                LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

                // تعيين بعض الخصائص الأساسية
                label.Caption = "Sample Label";

                // الوصول إلى خاصية Font (للقراءة فقط)
                Font controlFont = label.Font;

                // اعرض خصائص الخط
                Console.WriteLine("Font Name: " + controlFont.Name);
                Console.WriteLine("Font Size: " + controlFont.Size);
                Console.WriteLine("Is Bold: " + controlFont.IsBold);
                Console.WriteLine("Is Italic: " + controlFont.IsItalic);
                Console.WriteLine("Color: " + controlFont.Color);
                Console.WriteLine("Underline Type: " + controlFont.Underline);

                // احفظ المصنف
                workbook.Save("FontDemo.xlsx");
                Console.WriteLine("Font properties demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Font](../../../aspose.cells/font/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


