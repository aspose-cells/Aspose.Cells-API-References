---
title: "OoxmlSaveOptions.CompressionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OoxmlSaveOptions. Ottiene e imposta il tipo di compressione per il file ooxml"
type: docs
url: /it/net/aspose.cells/ooxmlsaveoptions/compressiontype/
---
## OoxmlSaveOptions.CompressionType property

Ottiene e imposta il tipo di compressione per il file ooxml.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Osservazioni

Il valore predefinito è OoxmlCompressionType.Level2.

### Esempi

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

### Vedi anche

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


