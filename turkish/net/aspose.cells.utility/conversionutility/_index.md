---
title: "Sınıf ConversionUtility"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Utility.ConversionUtility sınıfı. Dosyaları diğer formatlara dönüştürmek için bir yardımcı programı temsil eder."
type: docs
url: /tr/net/aspose.cells.utility/conversionutility/
---
## ConversionUtility class

Dosyaları diğer formatlara dönüştürmek için yardımcı aracı temsil eder.

```csharp
public class ConversionUtility
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert_1)(string, string) | Excel dosyalarını diğer formatlara dönüştürür. |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert)(string, LoadOptions, string, SaveOptions) | Excel dosyalarını diğer formatlara dönüştürür. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;
    using System.IO;

    public class UtilityClassConversionUtilityDemo
    {
        public static void Run()
        {
            // Dönüştürme için örnek bir CSV dosyası oluşturun
            string sourceFile = "sample.csv";
            string outputFile = "converted.xlsx";

            try
            {
                // Örnek CSV içeriği oluşturun
                File.WriteAllText(sourceFile, "Product,Price,Quantity\nApple,1.50,100\nBanana,0.75,150\nOrange,1.25,120");

                // Statik dönüşüm yöntemi kullanarak CSV'yi XLSX'e dönüştürün
                ConversionUtility.Convert(sourceFile, outputFile);

                Console.WriteLine($"Successfully converted {sourceFile} to {outputFile}");

                // Çıktı dosyasının var olup olmadığını kontrol ederek dönüşümü doğrulayın
                if (File.Exists(outputFile))
                {
                    Console.WriteLine("Output file created successfully");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Geçici dosyaları temizleyin
                if (File.Exists(sourceFile))
                {
                    File.Delete(sourceFile);
                }
                if (File.Exists(outputFile))
                {
                    File.Delete(outputFile);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


