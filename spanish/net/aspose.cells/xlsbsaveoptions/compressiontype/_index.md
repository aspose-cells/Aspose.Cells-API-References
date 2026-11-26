---
title: "XlsbSaveOptions.CompressionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XlsbSaveOptions. Obtiene y establece el tipo de compresión para el archivo ooxml"
type: docs
url: /es/net/aspose.cells/xlsbsaveoptions/compressiontype/
---
## XlsbSaveOptions.CompressionType property

Obtiene y establece el tipo de compresión para el archivo ooxml.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Observaciones

El valor predeterminado es OoxmlCompressionType.Level6.

### Ejemplos

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

### Ver también

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


