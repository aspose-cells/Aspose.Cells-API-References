---
title: "XlsbSaveOptions.CompressionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XlsbSaveOptions. Ottiene e imposta il tipo di compressione per il file ooxml"
type: docs
url: /it/net/aspose.cells/xlsbsaveoptions/compressiontype/
---
## XlsbSaveOptions.CompressionType property

Ottiene e imposta il tipo di compressione per il file ooxml.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Osservazioni

Il valore predefinito è OoxmlCompressionType.Level6.

### Esempi

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

### Vedi anche

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


