---
title: "OoxmlSaveOptions.CompressionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OoxmlSaveOptions. تحصل وتحدد نوع الضغط لملف ooxml"
type: docs
url: /ar/net/aspose.cells/ooxmlsaveoptions/compressiontype/
---
## OoxmlSaveOptions.CompressionType property

يحصل أو يضبط نوع الضغط لملف ooxml.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### ملاحظات

القيمة الافتراضية هي OoxmlCompressionType.Level2.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyCompressionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Compression Test");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());

            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6;

            workbook.Save("CompressionDemo.xlsx", saveOptions);
            Console.WriteLine("Workbook saved with Level6 compression.");
        }
    }
}
```

### انظر أيضًا

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


