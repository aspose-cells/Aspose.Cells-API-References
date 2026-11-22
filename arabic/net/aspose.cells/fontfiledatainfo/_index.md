---
title: "الفئة FontFileDataInfo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.FontFileDataInfo. تمثل معلومات بيانات ملف الخط"
type: docs
url: /ar/net/aspose.cells/fontfiledatainfo/
---
## FontFileDataInfo class

يمثل معلومات البيانات لملف الخط.

```csharp
public class FontFileDataInfo
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Data](../../aspose.cells/fontfiledatainfo/data/) { get; } | يحصل على البيانات الثنائية لملف الخط. |
| [FormatType](../../aspose.cells/fontfiledatainfo/formattype/) { get; } | يحصل على نوع تنسيق الخط لملف الخط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassFontFileDataInfoDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // مثال: تحميل بيانات ملف الخط
            string fontFilePath = "arial.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // ملاحظة: لا يمكن إنشاء كائن FontFileDataInfo مباشرةً لأنه لا يحتوي على مُنشئ عام
            // وخصائصه للقراءة فقط. في سيناريو واقعي، ستحصل على مثال
            // من طريقة API أخرى (مثل FontConfigs.GetFontFileDataInfo())
            FontFileDataInfo fontInfo = null; // Would be populated by API call in real scenario

            // عرض كيفية استخدام الخصائص إذا كان لدينا مثال
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
                Console.WriteLine("Font data length: " + (fontInfo.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            }

            // عرض التكامل مع Workbook
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // احفظ المصنف
            workbook.Save("FontFileDataInfoDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


