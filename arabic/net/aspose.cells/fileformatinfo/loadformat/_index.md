---
title: "FileFormatInfo.LoadFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FileFormatInfo. يحصل على تنسيق التحميل المكتشف"
type: docs
url: /ar/net/aspose.cells/fileformatinfo/loadformat/
---
## FileFormatInfo.LoadFormat property

يحصل على تنسيق التحميل المكتشف.

```csharp
public LoadFormat LoadFormat { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // المسار إلى دليل المستندات.
            string filePath = "data/";
            
            // اكتشف تنسيق الملف
            string fileName = "SAMPLE_XLS_ISSUE.XLS";
            var fileFormatInfo = FileFormatUtil.DetectFileFormat(filePath + fileName);
            Console.WriteLine("Detected LoadFormat: " + fileFormatInfo.LoadFormat);

            // حمّل الملف بالتنسيق الصحيح
            LoadOptions loadOptions = new LoadOptions(LoadFormat.MHtml);
            var workbook = new Workbook(filePath + fileName, loadOptions);
            
            // معالجة المصنف
            workbook.Worksheets[0].AutoFitColumns();
            workbook.Save(filePath + "output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [LoadFormat](../../loadformat/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


