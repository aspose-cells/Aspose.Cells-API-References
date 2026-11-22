---
title: "FillFormat.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FillFormat. تحصّل وتضبط نوع التعبئة"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/type/
---
## FillFormat.Type property

تحصّل وتضبط نوع التعبئة.

```csharp
[Obsolete("Use FillFormat.FillType  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FillType Type { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية FillFormat.FillType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2016. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
            FillFormat fill = shape.Fill;

            // اعرض قيمة Type الحالية
            Console.WriteLine("Current Type value: " + fill.Type);

            // غيّر Type إلى Gradient (خاصية غير صالحة تُستخدم للتوضيح)
            fill.Type = FillType.Gradient;

            // طبق تأثير تدرج لوني ثنائي
            fill.SetTwoColorGradient(Color.Blue, Color.Green, GradientStyleType.Horizontal, 1);

            // احفظ المصنف المعدل
            workbook.Save("FillFormatTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


