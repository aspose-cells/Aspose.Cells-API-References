---
title: "SpreadsheetML2003SaveOptions.IsIndentedFormatting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SpreadsheetML2003SaveOptions özelliği. Alt öğelerin girintili olmasını sağlar"
type: docs
url: /tr/net/aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/
---
## SpreadsheetML2003SaveOptions.IsIndentedFormatting property

Alt öğelerin girintili olmasını sağlar.

```csharp
public bool IsIndentedFormatting { get; set; }
```

### Açıklamalar

Varsayılan değer true'dur. Değer false ise, xml dosyasının boyutunu azaltır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyIsIndentedFormattingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Kaydetme seçeneklerini girintili biçimlendirme ile yapılandırın
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions
            {
                IsIndentedFormatting = true
            };

            // Girintili XML biçimlendirme ile kaydedin
            workbook.Save("output_indented.xml", saveOptions);

            // Karşılaştırma için girintili biçimlendirme olmadan kaydedin
            saveOptions.IsIndentedFormatting = false;
            workbook.Save("output_not_indented.xml", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


