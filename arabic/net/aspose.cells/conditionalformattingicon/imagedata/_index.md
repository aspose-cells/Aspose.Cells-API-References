---
title: "ConditionalFormattingIcon.ImageData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConditionalFormattingIcon. يحصل على بيانات مجموعة الأيقونات"
type: docs
url: /ar/net/aspose.cells/conditionalformattingicon/imagedata/
---
## ConditionalFormattingIcon.ImageData property

يحصل على بيانات مجموعة الأيقونات.

```csharp
public byte[] ImageData { get; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyImageDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة وتنسيق شرطي
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // احصل على نتيجة التنسيق الشرطي
            var conditionalFormattingResult = worksheet.Cells["A1"].GetConditionalFormattingResult();
            if (conditionalFormattingResult != null)
            {
                ConditionalFormattingIcon icon = conditionalFormattingResult.ConditionalFormattingIcon;
                if (icon != null)
                {
                    // احصل على بيانات صورة الأيقونة
                    byte[] imageData = icon.ImageData;
                    
                    // تحقق واعرض معلومات الصورة
                    if (imageData != null && imageData.Length > 0)
                    {
                        Console.WriteLine($"Icon data length: {imageData.Length} bytes");
                    }
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


