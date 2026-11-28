---
title: "Range.ClearComments"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Bu aralığın yorumlarını temizler"
type: docs
url: /tr/net/aspose.cells/range/clearcomments/
---
## Range.ClearComments method

Bu aralığın yorumlarını temizler.

```csharp
public void ClearComments()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere bazı veri ve yorumlar ekle
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A1"].PutValue("This is a comment on A1", true, false);
            worksheet.Cells["B2"].Value = "More Data";
            worksheet.Cells["B2"].PutValue("This is a comment on B2", true, false);

            try
            {
                // Yorumlu hücreleri içeren bir aralık oluştur
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Aralıktaki yorumları temizle
                range.ClearComments();

                Console.WriteLine("Comments cleared successfully from range A1:B2");
                Console.WriteLine($"Cell A1 value after clearing: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"Cell B2 value after clearing: {worksheet.Cells["B2"].Value}");

                // Çalışma kitabını kaydedin
                workbook.Save("ClearCommentsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ClearComments: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


