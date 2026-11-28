---
title: "Range.Union"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. İki aralığın birleşimini döndürür"
type: docs
url: /tr/net/aspose.cells/range/union/
---
## Range.Union method

İki aralığın birleşimini döndürür.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList Union(Range range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | Aralık | Aralık |

### Dönüş Değeri

İki aralığın birleşimi.

### Açıklamalar

NOTE: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Range.UnionRanges() yöntemini kullanın. Bu yöntem Kasım 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Birleşimi göstermek için iki aralık oluşturun
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:C3");

            // Aralıkları bazı verilerle doldurun
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");

            try
            {
                // Union yöntemini çağırın (not: bu eski sürümdür)
                ArrayList unionResult = range1.Union(range2);

                Console.WriteLine("Union method executed successfully");
                Console.WriteLine($"Number of ranges in union: {unionResult.Count}");

                // Birleşimdeki tüm aralıkların adreslerini gösterin
                foreach (Aspose.Cells.Range r in unionResult)
                {
                    Console.WriteLine($"Union range address: {r.Address}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("RangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


