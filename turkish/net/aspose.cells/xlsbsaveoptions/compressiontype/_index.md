---
title: "XlsbSaveOptions.CompressionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XlsbSaveOptions özelliği. ooxml dosyası için sıkıştırma tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/xlsbsaveoptions/compressiontype/
---
## XlsbSaveOptions.CompressionType property

ooxml dosyası için sıkıştırma türünü alır ve ayarlar.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Açıklamalar

Varsayılan değer OoxmlCompressionType.Level6'dır.

### Örnekler

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

### Ayrıca Bakınız

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


