---
title: "FileFormatUtil.SaveFormatToExtension"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FileFormatUtil yöntemi. Bir kaydetme biçimi enum değerini dosya uzantısına dönüştürür."
type: docs
url: /tr/net/aspose.cells/fileformatutil/saveformattoextension/
---
## FileFormatUtil.SaveFormatToExtension method

Kaydetme formatı enum değerini dosya uzantısına dönüştürür.

```csharp
public static string SaveFormatToExtension(SaveFormat format)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| biçim | SaveFormat | Kaydetme biçimi. |

### Dönüş Değeri

Döndürülen uzantı, başında nokta olan küçük harfli bir dizedir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodSaveFormatToExtensionWithSaveFormatDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test content");

            // Farklı biçimlerle SaveFormatToExtension'ı gösterin
            SaveOptions[] saveOptions = {
                new PdfSaveOptions(),
                new XlsSaveOptions(SaveFormat.Excel97To2003),
                new OoxmlSaveOptions(SaveFormat.Xlsx),
                new OdsSaveOptions()
            };

            foreach (var options in saveOptions)
            {
                string extension = FileFormatUtil.SaveFormatToExtension(options.SaveFormat);
                Console.WriteLine($"SaveFormat: {options.SaveFormat} -> Extension: {extension}");
                
                // Algılanan uzantıyla kaydet
                string fileName = $"output{extension}";
                workbook.Save(fileName, options);
                Console.WriteLine($"Saved file: {fileName}");
            }

            workbook.Dispose();
        }
    }
}
```

### Ayrıca Bakınız

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


