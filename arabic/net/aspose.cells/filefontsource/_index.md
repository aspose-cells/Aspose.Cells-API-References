---
title: "الفئة FileFontSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.FileFontSource فئة. تمثل ملف الخط TrueType الفردي المخزن في نظام الملفات"
type: docs
url: /ar/net/aspose.cells/filefontsource/
---
## FileFontSource class

يمثل ملف TrueType الخط الفردي المخزن في نظام الملفات.

```csharp
public class FileFontSource : FontSourceBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [FileFontSource](filefontsource/)(string) | منشئ. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FilePath](../../aspose.cells/filefontsource/filepath/) { get; } | مسار ملف الخط. |
| override [Type](../../aspose.cells/filefontsource/type/) { get; } | يرجع نوع مصدر الخط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFontSourceDemo
    {
        public static void FileFontSourceExample()
        {
            // حدد مسار ملف الخط TrueType
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";

            // إنشاء كائن FileFontSource
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            // عرض نوع مصدر الخط ومسار الملف
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // تعيين قيمة خلية
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Hello, Aspose!");

            // تطبيق الخط المخصص على الخلية
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont"; // Use the name of the font
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("FileFontSourceExample.xlsx");
            workbook.Save("FileFontSourceExample.pdf");
        }
    }
}
```

### انظر أيضًا

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


