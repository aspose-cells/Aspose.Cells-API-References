---
title: "الفئة MemoryFontSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.MemoryFontSource. يمثل ملف TrueType واحد مخزن في الذاكرة"
type: docs
url: /ar/net/aspose.cells/memoryfontsource/
---
## MemoryFontSource class

يمثل ملف TrueType واحد مخزن في الذاكرة.

```csharp
public class MemoryFontSource : FontSourceBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [MemoryFontSource](memoryfontsource/)(byte[]) | منشئ. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FontData](../../aspose.cells/memoryfontsource/fontdata/) { get; } | بيانات الخط الثنائية. |
| override [Type](../../aspose.cells/memoryfontsource/type/) { get; } | يرجع نوع مصدر الخط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassMemoryFontSourceDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحميل ملف خط TrueType إلى الذاكرة
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // إنشاء نسخة من MemoryFontSource باستخدام بيانات الخط
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // إنشاء مصفوفة مصادر الخط التي تحتوي على مصدر الخط في الذاكرة الخاص بنا
            FontSourceBase[] fontSources = new FontSourceBase[] { memoryFontSource };

            // تعيين مصادر الخط باستخدام FontConfigs
            FontConfigs.SetFontSources(fontSources);

            // استخدام الخط المخصص في خلية
            worksheet.Cells["A1"].PutValue("Text with custom font from memory");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);

            // احفظ المصنف
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


