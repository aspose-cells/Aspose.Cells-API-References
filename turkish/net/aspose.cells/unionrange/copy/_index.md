---
title: "UnionRange.Copy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange yöntemi. Yapıştırma özel seçenekleriyle aralığı kopyalama"
type: docs
url: /tr/net/aspose.cells/unionrange/copy/
---
## UnionRange.Copy method

Aralığı özel yapıştırma seçenekleriyle kopyalama.

```csharp
public void Copy(UnionRange range, PasteOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | UnionRange | Kaynak aralık. |
| seçenekler | PasteOptions | Yapıştırma özel seçenekleri. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodCopyWithUnionRangePasteOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["B1"].PutValue("Value1");
            worksheet.Cells["A2"].PutValue("More Data");
            worksheet.Cells["B2"].PutValue("Value2");

            try
            {
                // Kaynak UnionRange oluşturun
                UnionRange sourceRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

                // Hedef UnionRange oluşturun
                UnionRange destinationRange = worksheet.Cells.CreateRange("D1:E2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("D1:E2") });

                // Belirli ayarlarla PasteOptions oluşturun
                PasteOptions options = new PasteOptions();
                options.PasteType = PasteType.All;
                options.SkipBlanks = true;
                options.Transpose = false;

                // Copy yöntemini çağırın
                sourceRange.Copy(destinationRange, options);

                Console.WriteLine("Copy method executed successfully");
                Console.WriteLine($"Destination range: {destinationRange.RefersTo}");

                // Çalışma kitabını kaydedin
                workbook.Save("UnionRangeCopyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Copy: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PasteOptions](../../pasteoptions/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


