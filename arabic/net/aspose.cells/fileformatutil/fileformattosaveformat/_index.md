---
title: "FileFormatUtil.FileFormatToSaveFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FileFormatUtil. تحويل تنسيق الملف إلى تنسيق الحفظ"
type: docs
url: /ar/net/aspose.cells/fileformatutil/fileformattosaveformat/
---
## FileFormatUtil.FileFormatToSaveFormat method

تحويل تنسيق الملف إلى تنسيق حفظ.

```csharp
public static SaveFormat FileFormatToSaveFormat(FileFormatType format)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تنسيق | FileFormatType | نوع تنسيق الملف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodFileFormatToSaveFormatWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test FileFormatToSaveFormat");

            // احصل على نوع تنسيق الملف لدفتر العمل
            FileFormatType originalFormat = workbook.FileFormat;

            // تحويل FileFormatType إلى SaveFormat
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(originalFormat);

            // احفظ دفتر العمل باستخدام SaveFormat المحول
            string outputPath = "Output_" + saveFormat.ToString() + ".xlsx";
            workbook.Save(outputPath, saveFormat);

            Console.WriteLine("File saved successfully with SaveFormat: " + saveFormat);
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../saveformat/)
* enum [FileFormatType](../../fileformattype/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


