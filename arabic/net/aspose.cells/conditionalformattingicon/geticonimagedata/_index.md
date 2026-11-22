---
title: "ConditionalFormattingIcon.GetIconImageData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ConditionalFormattingIcon. الحصول على بيانات مجموعة الأيقونات"
type: docs
url: /ar/net/aspose.cells/conditionalformattingicon/geticonimagedata/
---
## ConditionalFormattingIcon.GetIconImageData method

احصل على بيانات مجموعة الأيقونات

```csharp
public static byte[] GetIconImageData(IconSetType type, int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | IconSetType | نوع الأيقونة |
| فهرس | Int32 | فهرس الأيقونة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class ConditionalFormattingIconMethodGetIconImageDataWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // لا حاجة لإنشاء نسخة لأن GetIconImageData ثابت
            
            try
            {
                // استدعِ GetIconImageData باستخدام IconSetType.Arrows3 والفهرس 0
                byte[] imageData = ConditionalFormattingIcon.GetIconImageData(IconSetType.Arrows3, 0);
                
                Console.WriteLine("Method executed successfully. Image data length: " + imageData.Length);
                
                // احفظ بيانات الصورة إلى ملف للتوضيح
                File.WriteAllBytes("icon_image.png", imageData);
                Console.WriteLine("Icon image saved to icon_image.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetIconImageData method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("ConditionalFormattingIconGetIconImageDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


