---
title: "XlsbSaveOptions.CompressionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XlsbSaveOptions-Eigenschaft. Liest und setzt den Kompressionstyp für ooxml-Dateien"
type: docs
url: /de/net/aspose.cells/xlsbsaveoptions/compressiontype/
---
## XlsbSaveOptions.CompressionType property

Liest und setzt den Kompressionstyp für ooxml-Datei.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Hinweise

Der Standardwert ist OoxmlCompressionType.Level6.

### Beispiele

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

### Siehe auch

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


