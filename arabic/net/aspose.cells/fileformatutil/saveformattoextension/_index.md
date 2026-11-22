---
title: "FileFormatUtil.SaveFormatToExtension"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FileFormatUtil. تحول قيمة تعداد تنسيق الحفظ إلى امتداد ملف"
type: docs
url: /ar/net/aspose.cells/fileformatutil/saveformattoextension/
---
## FileFormatUtil.SaveFormatToExtension method

يحول قيمة تعداد تنسيق الحفظ إلى امتداد ملف.

```csharp
public static string SaveFormatToExtension(SaveFormat format)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تنسيق | SaveFormat | تنسيق الحفظ. |

### قيمة الإرجاع

الامتداد المرجع هو سلسلة بحروف صغيرة مع نقطة في البداية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodSaveFormatToExtensionWithSaveFormatDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test content");

            // عرض SaveFormatToExtension مع صيغ مختلفة
            SaveOptions[] saveOptions = {
                new PdfSaveOptions(),
                new XlsSaveOptions(SaveFormat.Excel97To2003),
                new OoxmlSaveOptions(SaveFormat.Xlsx),
                new OdsSaveOptions()
            };

            foreach (var options in saveOptions)
            {
                string extension = FileFormatUtil.SaveFormatToExtension(options.SaveFormat);
                Console.WriteLine($"SaveFormat: {options.SaveFormat} -> Extension: {extension}");
                
                // احفظ باستخدام الامتداد المكتشف
                string fileName = $"output{extension}";
                workbook.Save(fileName, options);
                Console.WriteLine($"Saved file: {fileName}");
            }

            workbook.Dispose();
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


