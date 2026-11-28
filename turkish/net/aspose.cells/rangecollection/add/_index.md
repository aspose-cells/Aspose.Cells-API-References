---
title: "RangeCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RangeCollection yöntemi. Bir Range öğesini koleksiyona ekler"
type: docs
url: /tr/net/aspose.cells/rangecollection/add/
---
## RangeCollection.Add method

Koleksiyona bir [`Range`](../../range/) öğesi ekler.

```csharp
[Obsolete("Use RangeCollection.AddRange(Range) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(Range range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | Aralık | Range nesnesi |

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen AddRange() yöntemini kullanın. Bu yöntem, Aralık 2025'ten itibaren 6 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionMethodAddWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir Range oluştur ve koleksiyona ekle
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Range'in genişlediğini göstermek için satırlar ekle
            worksheet.Cells.InsertRows(2, 2);
            
            Console.WriteLine("Range row count after insertion: " + cellRange.RowCount);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


