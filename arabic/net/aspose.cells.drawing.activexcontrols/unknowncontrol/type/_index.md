---
title: "UnknownControl.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية UnknownControl. تحصل على نوع عنصر التحكم ActiveX"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/unknowncontrol/type/
---
## UnknownControl.Type property

يحصل على نوع عنصر التحكم ActiveX.

```csharp
public override ControlType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlPropertyTypeDemo
    {
        public static void Run()
        {
            // تحميل دفتر عمل موجود يحتوي على عنصر تحكم غير معروف
            Workbook workbook = new Workbook("input_with_unknown_control.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            // العثور على ومعالجة مثيلات UnknownControl
            foreach (Shape shape in worksheet.Shapes)
            {
                if (shape.ActiveXControl is UnknownControl control)
                {
                    // عرض قراءة خاصية Type
                    Console.WriteLine($"Found control with Type: {control.Type}");
                    
                    // مثال على الاستخدام بناءً على نوع العنصر
                    if (control.Type == ControlType.ListBox)
                    {
                        Console.WriteLine("Processing legacy ListBox control");
                    }
                    else if (control.Type == ControlType.Unknown)
                    {
                        Console.WriteLine("Handling completely unknown control type");
                    }
                }
            }

            // حفظ دفتر العمل المعالج
            workbook.Save("ControlTypeAnalysis.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlType](../../controltype/)
* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


