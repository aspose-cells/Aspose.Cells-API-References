---
title: "Range.UnionRanges"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. İki aralığın birleşim sonucunu döndürür"
type: docs
url: /tr/net/aspose.cells/range/unionranges/
---
## Range.UnionRanges method

İki aralığın birleşim sonucunu döndürür.

```csharp
public UnionRange UnionRanges(Range[] ranges)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralıklar | Range[] | Aralık |

### Dönüş Değeri

İki aralığın birleşimi.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodUnionRangesWithRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelerde örnek veri oluştur
            worksheet.Cells["A1"].PutValue("Range 1");
            worksheet.Cells["B1"].PutValue("Data 1");
            worksheet.Cells["C1"].PutValue("Data 2");
            worksheet.Cells["A5"].PutValue("Range 2");
            worksheet.Cells["B5"].PutValue("Data 3");
            worksheet.Cells["C5"].PutValue("Data 4");

            // Birleştirilecek aralıklar oluştur
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A5:C7");

            try
            {
                // Range[] parametresiyle UnionRanges'ı çağır
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range1, range2 };
                UnionRange unionRange = range1.UnionRanges(rangesToUnion);

                // Birleşik aralığı göstermek için stil uygula
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });

                Console.WriteLine($"Union range created successfully. Address: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRanges method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("UnionRangesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../../unionrange/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


