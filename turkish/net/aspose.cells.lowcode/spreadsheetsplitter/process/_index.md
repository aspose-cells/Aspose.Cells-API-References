---
title: "SpreadsheetSplitter.Process"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SpreadsheetSplitter metodu. Verilen şablon dosyasını birden çok parçaya böler"
type: docs
url: /tr/net/aspose.cells.lowcode/spreadsheetsplitter/process/
---
## Process(string, string) {#process_1}

Verilen şablon dosyasını birden çok parçaya böler.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| templateFile | String | Bölünecek şablon dosyası |
| resultFile | String | Sonuç dosyası (ad deseni) |

### Açıklamalar

Çıktı dosyaları, sayfa ve bölünmüş parça sıra numarası eklenerek belirtilen sonuç dosyasından oluşturulacaktır. Örneğin, belirtilen çıktı dosyası Split.xlsx ise, oluşturulan dosyalar Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ... şeklinde olacaktır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetSplitterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Birden fazla çalışma sayfasına sahip yeni bir çalışma kitabı oluşturun
            Workbook templateWorkbook = new Workbook();
            Worksheet sheet1 = templateWorkbook.Worksheets.Add("SalesData");
            sheet1.Cells["A1"].PutValue("Product");
            Worksheet sheet2 = templateWorkbook.Worksheets.Add("Inventory");
            sheet2.Cells["A1"].PutValue("test data");

            // Şablon dosyası olarak kaydet
            string templatePath = "SplitterTemplate.xlsx";
            templateWorkbook.Save(templatePath, SaveFormat.Xlsx);

            // Sonuç çıktı desenini tanımlayın
            string resultPattern = "SplitResult_";
            
            try
            {
                // Şablonu doğrudan statik yöntemle işleyin
                SpreadsheetSplitter.Process(templatePath, resultPattern);
                
                Console.WriteLine($"Spreadsheet split successfully using pattern: {resultPattern}");
                Console.WriteLine("Check output directory for split files");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during spreadsheet splitting: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeSplitOptions) {#process}

Elektronik tablo dosyasını birden fazla parçaya böler.

```csharp
public static void Process(LowCodeSplitOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | LowCodeSplitOptions | Elektronik tabloyu bölmek için seçenekler |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetSplitterMethodProcessWithLowCodeSplitOptionsDemo
    {
        public static void Run()
        {

            // Bölme seçeneklerini başlat
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions
            {
                LoadOptions = new LowCodeLoadOptions { InputFile = "split.xlsx" },
                SaveOptionsProvider = new CustomLowCodeSaveOptionsProvider()
            };

            try
            {
                // Statik yöntem kullanarak elektronik tablo bölmeyi yürüt
                SpreadsheetSplitter.Process(splitOptions);
                
                Console.WriteLine($"Spreadsheet split successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Split operation failed: {ex.Message}");
            }
        }
    }

    // AbstractLowCodeSaveOptionsProvider'ın somut uygulaması
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        {
            base.Finish(part);
        }
        // Gerekli soyut yöntemi uygulayın
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSplitOptions](../../lowcodesplitoptions/)
* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


