---
title: "Enum OpenDocumentFormatVersionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Ods.OpenDocumentFormatVersionType enum. Open Document Format sürüm türü"
type: docs
url: /tr/net/aspose.cells.ods/opendocumentformatversiontype/
---
## OpenDocumentFormatVersionType enumeration

Open Document Format sürüm türü.

```csharp
public enum OpenDocumentFormatVersionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Sıkı olmayan. |
| Odf11 | `1` | ODF Sürüm 1.1 |
| Odf12 | `2` | ODF Sürüm 1.2 |
| Odf13 | `3` | ODF Sürüm 1.3 |
| Odf14 | `4` | ODF Sürüm 1.4 |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OpenDocumentFormatVersionTypeDemo
    {
        public static void OpenDocumentFormatVersionTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // OdsSaveOptions oluşturun ve ODF sürümünü ayarlayın
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Çalışma kitabını belirtilen ODF sürümüyle ODS formatında kaydedin
            workbook.Save("OpenDocumentFormatVersionTypeExample.ods", saveOptions);

            Console.WriteLine("Workbook saved successfully with ODF version 1.2.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


