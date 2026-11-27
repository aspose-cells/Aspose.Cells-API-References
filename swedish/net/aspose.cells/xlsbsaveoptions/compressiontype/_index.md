---
title: "XlsbSaveOptions.CompressionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XlsbSaveOptions-egenskap. Hämtar och anger kompressionstypen för ooxml-fil"
type: docs
url: /sv/net/aspose.cells/xlsbsaveoptions/compressiontype/
---
## XlsbSaveOptions.CompressionType property

Hämtar och anger komprimeringstypen för ooxml‑fil.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Anmärkningar

Standardvärdet är OoxmlCompressionType.Level6.

### Exempel

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

### Se även

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


