---
title: "ConversionUtility.Convert"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConversionUtility yöntemi. Excel dosyalarını diğer formatlara dönüştürür"
type: docs
url: /tr/net/aspose.cells.utility/conversionutility/convert/
---
## Convert(string, string) {#convert_1}

Excel dosyalarını diğer formatlara dönüştürür.

```csharp
public static void Convert(string source, string saveAs)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | String | Kaynak dosya adı. |
| saveAs | String | Beklenen dosyanın dosya adı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ConversionUtilityMethodConvertWithStringStringDemo
    {
        public static void Run()
        {
            // Kaynak ve hedef dosya yollarını başlat
            string sourcePath = "source.xlsx";
            string destPath = "output.pdf";
            // Excel dosyasını PDF'ye dönüştür
            ConversionUtility.Convert(sourcePath, destPath);

            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## Convert(string, LoadOptions, string, SaveOptions) {#convert}

Excel dosyalarını diğer formatlara dönüştürür.

```csharp
public static void Convert(string source, LoadOptions loadOptions, string saveAs, 
    SaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | String | Kaynak dosya adı. |
| loadOptions | LoadOptions | Kaynak dosyayı yükleme seçenekleri. |
| saveAs | String | Beklenen dosyanın dosya adı. |
| saveOptions | SaveOptions | Dosyayı kaydetme seçenekleri. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ConversionUtilityMethodConvertWithStringLoadOptionsStringSaveOptDemo
    {
        public static void Run()
        {
            // Kaynak ve hedef dosya yolları
            string sourceFile = "input.csv";
            string outputFile = "output.xlsx";

            // Demonstrasyon için örnek CSV dosyası oluştur
            System.IO.File.WriteAllText(sourceFile, "Name,Age\nJohn,30\nAlice,25");

            try
            {
                // CSV dosyası için yükleme seçenekleri oluştur
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                
                // XLSX dosyası için kaydetme seçenekleri oluştur
                SaveOptions saveOptions = new OoxmlSaveOptions();

                // Belirtilen seçeneklerle CSV'yi XLSX'ye dönüştür
                ConversionUtility.Convert(sourceFile, loadOptions, outputFile, saveOptions);

                Console.WriteLine($"File converted successfully from {sourceFile} to {outputFile}");
                
                // Çıktı dosyasını yükleyerek dönüşümü doğrula
                Workbook workbook = new Workbook(outputFile);
                Console.WriteLine($"Output file contains {workbook.Worksheets.Count} worksheet(s)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Geçici dosyaları temizleyin
                if (System.IO.File.Exists(sourceFile))
                {
                    System.IO.File.Delete(sourceFile);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../../../aspose.cells/loadoptions/)
* class [SaveOptions](../../../aspose.cells/saveoptions/)
* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


