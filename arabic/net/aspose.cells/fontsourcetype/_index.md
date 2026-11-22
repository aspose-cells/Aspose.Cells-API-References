---
title: "التعداد FontSourceType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.FontSourceType. يحدد نوع مصدر الخط"
type: docs
url: /ar/net/aspose.cells/fontsourcetype/
---
## FontSourceType enumeration

يحدد نوع مصدر الخط.

```csharp
public enum FontSourceType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| FontFile | `0` | يمثل ملف خط واحد. |
| FontsFolder | `1` | يمثل مجلدًا يحتوي على ملفات الخطوط. |
| MemoryFont | `2` | يمثل خطًا واحدًا في الذاكرة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontSourceTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // عرض قيم تعداد FontSourceType
            Console.WriteLine("FontSourceType values:");
            Console.WriteLine($"FontFile: {FontSourceType.FontFile}");
            Console.WriteLine($"FontsFolder: {FontSourceType.FontsFolder}");
            Console.WriteLine($"MemoryFont: {FontSourceType.MemoryFont}");

            // إنشاء إعدادات الخط واستخدام FontSourceType
            FontConfigs.SetFontFolder(@"C:\MyFonts\", false);
            FontConfigs.SetFontSources(new FontSourceBase[]
            {
                new FolderFontSource(@"C:\MyFonts\", false),
                new FileFontSource(@"C:\MyFonts\arial.ttf"),
                new MemoryFontSource(new byte[0])
            });

            // تطبيق الخط على خلية
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with Arial font");

            // حفظ النتيجة
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


