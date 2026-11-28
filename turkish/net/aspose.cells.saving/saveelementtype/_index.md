---
title: "Enum SaveElementType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Saving.SaveElementType enum. Hangi tür öğelerin kaydedilmesi gerektiğini temsil eder"
type: docs
url: /tr/net/aspose.cells.saving/saveelementtype/
---
## SaveElementType enumeration

Hangi tür öğelerin kaydedilmesi gerektiğini temsil eder.

```csharp
public enum SaveElementType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| All | `251658239` | Tüm veri. |
| Chart | `256` | Yalnızca grafikler. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassSaveElementTypeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Kaydetmeyi göstermek için bazı örnek veriler ekle
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["B1"].PutValue(12345);

                // Chart kaydetme öğesi türünü göstermek için bir grafik oluştur
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B1", true);

                // SaveElementType enum değerlerini kullanarak göster
                SaveElementType chartType = SaveElementType.Chart;
                SaveElementType allType = SaveElementType.All;

                Console.WriteLine($"Chart SaveElementType value: {chartType}");
                Console.WriteLine($"All SaveElementType value: {allType}");

                // Çalışma kitabını tüm öğelerle kaydet
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                workbook.Save("SaveElementTypeDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully with all elements");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SaveElementType: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


