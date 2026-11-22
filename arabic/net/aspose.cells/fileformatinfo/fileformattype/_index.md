---
title: "FileFormatInfo.FileFormatType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FileFormatInfo. يحصل على تنسيق الملف المكتشف"
type: docs
url: /ar/net/aspose.cells/fileformatinfo/fileformattype/
---
## FileFormatInfo.FileFormatType property

يحصل على تنسيق الملف المكتشف.

```csharp
public FileFormatType FileFormatType { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // مثال 1: اكتشف تنسيق Excel 97-2003
            string excelFile = "sample.xls";
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(excelFile);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            Console.WriteLine("Is Encrypted: " + info.IsEncrypted);

            // مثال 2: اكتشف تنسيق OOXML
            string xlsxFile = "sample.xlsx";
            info = FileFormatUtil.DetectFileFormat(xlsxFile);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            Console.WriteLine("Is Encrypted: " + info.IsEncrypted);
        }
    }
}
```

### انظر أيضًا

* enum [FileFormatType](../../fileformattype/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


