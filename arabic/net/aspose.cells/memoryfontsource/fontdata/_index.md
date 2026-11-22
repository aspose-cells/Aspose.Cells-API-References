---
title: "MemoryFontSource.FontData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MemoryFontSource. بيانات الخط الثنائية"
type: docs
url: /ar/net/aspose.cells/memoryfontsource/fontdata/
---
## MemoryFontSource.FontData property

بيانات الخط الثنائية.

```csharp
public byte[] FontData { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourcePropertyFontDataDemo
    {
        public static void Run()
        {
            // تحميل ملف خط TrueType إلى الذاكرة
            byte[] fontBytes = File.ReadAllBytes("arial.ttf");

            // إنشاء كائن MemoryFontSource باستخدام بيانات الخط
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontBytes);

            // عرض قيمة FontData الحالية (أول 10 بايت للتوضيح)
            Console.WriteLine("FontData length: " + memoryFontSource.FontData.Length);
            Console.Write("First 10 bytes: ");
            for (int i = 0; i < 10 && i < memoryFontSource.FontData.Length; i++)
            {
                Console.Write(memoryFontSource.FontData[i].ToString("X2") + " ");
            }
            Console.WriteLine();

            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء إعدادات الخط وإضافة مصدر الخط الذاكرة الخاص بنا
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // تطبيق إعدادات الخط عالميًا (ليس خاصًا بالدفتر)
            FontConfigs.DefaultFontName = "Arial";
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // إنشاء نمط باستخدام الخط المخصص
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;

            // تطبيق النمط على خلية
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text using memory font source");

            // احفظ المصنف
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


