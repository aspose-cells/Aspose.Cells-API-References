---
title: "MemoryFontSource.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MemoryFontSource. تُرجع نوع مصدر الخط"
type: docs
url: /ar/net/aspose.cells/memoryfontsource/type/
---
## MemoryFontSource.Type property

يرجع نوع مصدر الخط.

```csharp
public override FontSourceType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            // تحميل ملف خط TrueType إلى الذاكرة
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // إنشاء كائن MemoryFontSource باستخدام بيانات الخط
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // عرض قيمة Type الحالية
            Console.WriteLine("MemoryFontSource Type: " + memoryFontSource.Type);

            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين مصادر الخط باستخدام FontConfigs
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // تحقق من أن نوع مصدر الخط هو MemoryFont
            if (memoryFontSource.Type == FontSourceType.MemoryFont)
            {
                // استخدام الخط في خلية
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text using memory font source");

                // إضافة معلومات حول نوع مصدر الخط
                worksheet.Cells["A2"].PutValue("Font source type: " + memoryFontSource.Type);
            }

            // احفظ المصنف
            workbook.Save("MemoryFontSourceTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FontSourceType](../../fontsourcetype/)
* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


