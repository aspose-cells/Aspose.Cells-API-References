---
title: "MsoFormatPicture.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة MsoFormatPicture."
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/equals/
---
## MsoFormatPicture.Equals method

```csharp
public override bool Equals(object obj)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | Object |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPictureMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورتين إلى ورقة العمل
            int pictureIndex1 = worksheet.Pictures.Add(0, 0, "example.jpg");
            int pictureIndex2 = worksheet.Pictures.Add(5, 0, "example.jpg");
            
            Picture picture1 = worksheet.Pictures[pictureIndex1];
            Picture picture2 = worksheet.Pictures[pictureIndex2];

            // احصل على كائنات MsoFormatPicture
            MsoFormatPicture format1 = picture1.FormatPicture;
            MsoFormatPicture format2 = picture2.FormatPicture;

            // تعيين خصائص مختلفة لتوضيح مقارنة المساواة
            format1.Brightness = 0.5;
            format1.Contrast = 0.3;
            format2.Brightness = 0.5;
            format2.Contrast = 0.3;

            try
            {
                // قارن كائنَي MsoFormatPicture
                bool areEqual = format1.Equals((object)format2);
                Console.WriteLine($"Format objects are equal: {areEqual}");

                // عدّل تنسيقًا واحدًا وقارن مرة أخرى
                format2.Brightness = 0.7;
                areEqual = format1.Equals((object)format2);
                Console.WriteLine($"After modification, format objects are equal: {areEqual}");

                // قارن مع null
                bool isNullEqual = format1.Equals((object)null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // قارن مع نوع مختلف
                bool isDifferentTypeEqual = format1.Equals((object)"string");
                Console.WriteLine($"Comparison with different type: {isDifferentTypeEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("MsoFormatPictureMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


