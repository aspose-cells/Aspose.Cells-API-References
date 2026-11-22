---
title: "FillFormat.SetType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FillFormat. تحصّل على نوع تنسيق التعبئة المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/settype/
---
## FillFormat.SetType property

تحصّل على نوع تنسيق التعبئة المحدد.

```csharp
[Obsolete("Use FillFormat.FillType instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FormatSetType SetType { get; set; }
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

    public class FillFormatPropertySetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
            FillFormat fillFormat = shape.Fill;

            Console.WriteLine("Current SetType value: " + fillFormat.SetType);

            fillFormat.SetType = FormatSetType.IsGradientSet;
            fillFormat.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);

            Console.WriteLine("New SetType value: " + fillFormat.SetType);

            workbook.Save("FillFormatSetTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FormatSetType](../../formatsettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


