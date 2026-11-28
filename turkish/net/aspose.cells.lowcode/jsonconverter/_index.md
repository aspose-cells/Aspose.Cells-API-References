---
title: "Sınıf JsonConverter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.JsonConverter sınıfı. JSON veri yapısı ile diğer elektronik tablo dosya formatları arasında dönüşüm için dönüştürücü"
type: docs
url: /tr/net/aspose.cells.lowcode/jsonconverter/
---
## JsonConverter class

JSON veri yapısı ile diğer elektronik tablo dosya biçimleri arasında dönüşüm yapan dönüştürücü.

```csharp
public class JsonConverter
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | JSON verisi ile diğer elektronik tablo dosya formatları arasında dönüştürür. |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process_1)(string, string) | Verilen şablon dosyasını JSON ile diğer formatlar arasında dönüştürür. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassJsonConverterDemo
    {
        public static void Run()
        {
            string jsonFilePath = "data.json";
            string excelFilePath = "res.xlsx";

            try
            {
                // Aspose.Cells.LowCode.JsonConverter kullanarak JSON'u Excel'e dönüştürün
                JsonConverter.Process(jsonFilePath, excelFilePath);

                Console.WriteLine("Conversion completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


