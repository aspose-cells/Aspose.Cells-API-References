---
title: "OoxmlSaveOptions.CompressionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OoxmlSaveOptions. Obtiene y establece el tipo de compresión para el archivo ooxml"
type: docs
url: /es/net/aspose.cells/ooxmlsaveoptions/compressiontype/
---
## OoxmlSaveOptions.CompressionType property

Obtiene y establece el tipo de compresión para el archivo ooxml.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Observaciones

El valor predeterminado es OoxmlCompressionType.Level2.

### Ejemplos

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

### Ver también

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


