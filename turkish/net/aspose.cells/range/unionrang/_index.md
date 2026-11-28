---
title: "Range.UnionRang"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. İki aralığın birleşim sonucunu döndürür"
type: docs
url: /tr/net/aspose.cells/range/unionrang/
---
## Range.UnionRang method

İki aralığın birleşim sonucunu döndürür.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Range[] UnionRang(Range range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | Aralık | Aralık |

### Dönüş Değeri

İki aralığın birleşimi.

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine lütfen Range.UnionRanges() yöntemini kullanın. Bu yöntem Mayıs 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using Range = Aspose.Cells.Range; // Add this alias to resolve ambiguity

    public class RangeMethodUnionRangWithRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // UnionRang'i göstermek için iki aralık oluştur
            Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Range range2 = worksheet.Cells.CreateRange("C3:D4");

            // Görselleştirme için aralıklara bazı değerler ayarla
            range1[0, 0].PutValue("Range1");
            range1[1, 1].PutValue("Data");
            range2[0, 0].PutValue("Range2");
            range2[1, 1].PutValue("Data");

            try
            {
                // İki aralığı birleştirmek için UnionRang yöntemini çağır
                Range[] unionResult = range1.UnionRang(range2);

                // Birleşim sonucu hakkında bilgi göster
                Console.WriteLine("UnionRang method executed successfully.");
                Console.WriteLine($"Number of ranges in union: {unionResult.Length}");
                Console.WriteLine($"First union range address: {unionResult[0].Address}");
                Console.WriteLine($"Second union range address: {unionResult[1].Address}");

                // Görselleştirme için birleşim aralıklarını bir kenarlıkla işaretle
                foreach (Range r in unionResult)
                {
                    r.SetOutlineBorders(CellBorderType.Thin, System.Drawing.Color.Black);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRang method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("RangeMethodUnionRangWithRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


