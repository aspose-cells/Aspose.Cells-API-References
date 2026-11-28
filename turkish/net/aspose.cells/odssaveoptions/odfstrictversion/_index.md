---
title: "OdsSaveOptions.OdfStrictVersion"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OdsSaveOptions özelliği. ODF sürümünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/odssaveoptions/odfstrictversion/
---
## OdsSaveOptions.OdfStrictVersion property

ODF sürümünü alır ve ayarlar.

```csharp
public OpenDocumentFormatVersionType OdfStrictVersion { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyOdfStrictVersionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ODF Version Demo");

            // ODS kaydetme seçeneklerini oluştur
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            
            // ODF sürümünü 1.2 olarak ayarla
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Belirtilen ODF sürümüyle kaydet
            workbook.Save("OdfVersion12.ods", saveOptions);

            // ODF sürümünü 1.3'e değiştir
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf13;
            workbook.Save("OdfVersion13.ods", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


