---
title: "StyleFlag.Alignments"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد المحاذاة"
type: docs
url: /ar/net/aspose.cells/styleflag/alignments/
---
## StyleFlag.Alignments property

سيتم تطبيق إعداد المحاذاة.

```csharp
public bool Alignments { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyAlignmentsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية A1 وتعيين بعض النص
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // إنشاء كائن نمط وتعيين خصائص المحاذاة
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.RotationAngle = 45;

            // إنشاء علامة نمط وتمكين خصائص المحاذاة
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Alignments = true;

            // تطبيق النمط على الخلية باستخدام علم النمط
            cell.SetStyle(style, styleFlag);

            // عرض إعدادات المحاذاة الحالية
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // تعديل علامة النمط لتعطيل خصائص المحاذاة
            styleFlag.Alignments = false;
            
            // إنشاء نمط جديد بمحاذاة مختلفة
            Style newStyle = workbook.CreateStyle();
            newStyle.HorizontalAlignment = TextAlignmentType.Right;
            newStyle.VerticalAlignment = TextAlignmentType.Top;
            newStyle.RotationAngle = 0;

            // تطبيق النمط الجديد - لن تتغير المحاذاة لأن العلامة غير مفعلة
            cell.SetStyle(newStyle, styleFlag);

            // عرض إعدادات المحاذاة غير المتغيرة
            Console.WriteLine("After applying new style with Alignments=false:");
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // احفظ المصنف
            workbook.Save("StyleFlagAlignmentsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


