---
title: "UnionRange.ColumnCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange özelliği. Aralıktaki satır sayısını alır"
type: docs
url: /tr/net/aspose.cells/unionrange/columncount/
---
## UnionRange.ColumnCount property

Aralıktaki satır sayısını alır.

```csharp
public int ColumnCount { get; }
```

### Açıklamalar

Yalnızca bir aralık içerdiğinde etkili olur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Laptop";
            worksheet.Cells["B2"].Value = 1200;
            worksheet.Cells["C2"].Value = 5;
            worksheet.Cells["A3"].Value = "Phone";
            worksheet.Cells["B3"].Value = 800;
            worksheet.Cells["C3"].Value = 10;

            try
            {
                // Aralıklar oluşturun ve bunları bir birleşim aralığına birleştirin
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C2");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A3:C3");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // ColumnCount özelliği değerini göster
                Console.WriteLine("ColumnCount of union range: " + unionRange.ColumnCount);

                // Sütun bilgilerini göstererek kullanımını göster
                Console.WriteLine("First column index: " + unionRange.FirstColumn);
                Console.WriteLine("Last column index: " + (unionRange.FirstColumn + unionRange.ColumnCount - 1));

                // Farklı sütun sayısına sahip başka bir birleşik aralık oluştur
                Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("A1:B2");
                Aspose.Cells.Range range4 = worksheet.Cells.CreateRange("D1:E2");
                UnionRange unionRange2 = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range3, range4 });

                // Sütun sayılarını karşılaştır
                Console.WriteLine("Second union range ColumnCount: " + unionRange2.ColumnCount);
                Console.WriteLine("First union range has " +
                    (unionRange.ColumnCount > unionRange2.ColumnCount ? "more" : "fewer") +
                    " columns than second union range");

                // Çalışma kitabını kaydedin
                workbook.Save("UnionRangeColumnCountDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


