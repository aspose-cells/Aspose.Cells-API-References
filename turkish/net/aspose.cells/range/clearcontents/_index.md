---
title: "Range.ClearContents"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Bu aralığın içeriğini temizler"
type: docs
url: /tr/net/aspose.cells/range/clearcontents/
---
## Range.ClearContents method

Bu aralığın içeriğini temizler.

```csharp
public void ClearContents()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearContentsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Temizlemeyi göstermek için bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue("Sample");
            worksheet.Cells["B2"].PutValue("Data");

            try
            {
                // A1:B2 hücrelerini kapsayan bir aralık oluşturun
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Temizlemeden önce aralık içeriğini gösterin
                Console.WriteLine("Before clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Aralıktaki tüm değerleri kaldırmak için ClearContents metodunu çağırın
                range.ClearContents();

                // Temizledikten sonra aralık içeriğini gösterin
                Console.WriteLine("\nAfter clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Çalışma kitabını kaydedin
                workbook.Save("ClearContentsDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


