---
title: "FillFormat.FillType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FillFormat. يسترجع ويضبط نوع الملء"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/filltype/
---
## FillFormat.FillType property

يحصل على نوع التعبئة ويضبطه

```csharp
public FillType FillType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyFillTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // تعيين ملء صلب باللون
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Red;

            // إخراج نوع الملء
            Console.WriteLine("Shape fill type: " + shape.Fill.FillType);

            // تغيير إلى ملء تدرجي
            shape.Fill.FillType = FillType.Gradient;
            Console.WriteLine("Shape fill type changed to: " + shape.Fill.FillType);

            // احفظ المصنف
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


