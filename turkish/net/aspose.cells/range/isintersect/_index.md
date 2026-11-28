---
title: "Range.IsIntersect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Aralığın kesişip kesişmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/range/isintersect/
---
## Range.IsIntersect method

Aralığın kesişip kesişmediğini gösterir.

```csharp
public bool IsIntersect(Range range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | Aralık | Aralık. |

### Dönüş Değeri

Aralığın kesişip kesişmediği.

### Açıklamalar

İki aralık aynı çalışma sayfasında değilse, false döndür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodIsIntersectWithRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kesişmeyi test etmek için iki aralık oluştur
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B3:D8");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("C10:D15");

            try
            {
                // range1'in range2 ile kesişip kesişmediğini kontrol et (kesişmeli)
                bool result1 = range1.IsIntersect(range2);
                Console.WriteLine($"Range A1:B5 intersects with B3:D8: {result1}");

                // range1'in range3 ile kesişip kesişmediğini kontrol et (kesişmemeli)
                bool result2 = range1.IsIntersect(range3);
                Console.WriteLine($"Range A1:B5 intersects with C10:D15: {result2}");

                // Aralıkları farklı renklerle doldur ve görselleştir
                Style style1 = workbook.CreateStyle();
                style1.ForegroundColor = System.Drawing.Color.LightBlue;
                style1.Pattern = BackgroundType.Solid;
                range1.SetStyle(style1);

                Style style2 = workbook.CreateStyle();
                style2.ForegroundColor = System.Drawing.Color.LightGreen;
                style2.Pattern = BackgroundType.Solid;
                range2.SetStyle(style2);

                Style style3 = workbook.CreateStyle();
                style3.ForegroundColor = System.Drawing.Color.LightPink;
                style3.Pattern = BackgroundType.Solid;
                range3.SetStyle(style3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsIntersect method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("RangeMethodIsIntersectWithRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


