---
title: "XlsbSaveOptions.CompressionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XlsbSaveOptions. تحصل وتعيّن نوع الضغط لملف ooxml"
type: docs
url: /ar/net/aspose.cells/xlsbsaveoptions/compressiontype/
---
## XlsbSaveOptions.CompressionType property

يحصل أو يضبط نوع الضغط لملف ooxml.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### ملاحظات

القيمة الافتراضية هي OoxmlCompressionType.Level6.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyCompressionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Compression Test");

            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                CompressionType = OoxmlCompressionType.Level6
            };

            workbook.Save("XlsbWithCompression.xlsb", saveOptions);
        }
    }
}
```

### انظر أيضًا

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


