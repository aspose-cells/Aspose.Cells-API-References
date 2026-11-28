---
title: "Cells.MergedCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Birleştirilmiş hücrelerin koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/cells/mergedcells/
---
## Cells.MergedCells property

Birleştirilmiş hücrelerin koleksiyonunu alır.

```csharp
[Obsolete("Use Cells.GetMergedAreas() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList MergedCells { get; }
```

### Açıklamalar

Bu koleksiyonda, her öğe birleştirilmiş hücrelerin alanını temsil eden bir [`CellArea`](../../cellarea/) yapısıdır.

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Cells.GetMergedAreas() yöntemini kullanın. Bu yöntem Kasım 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsPropertyMergedCellsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // İki farklı aralıkta hücreleri birleştir
            cells.Merge(0, 0, 2, 2); // Merges A1:B2
            cells.Merge(2, 2, 2, 2); // Merges C3:D4

            // MergedCells özelliğine eriş (yalnızca okunabilir)
            ArrayList mergedRanges = cells.MergedCells;

            // İlk birleştirilmiş hücre sayısını ve aralıklarını göster
            Console.WriteLine($"Initial merged cells count: {mergedRanges.Count}");
            foreach (CellArea area in mergedRanges)
            {
                Console.WriteLine($"Merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // İlk birleştirilmiş aralığı birleştirmeyi kaldır
            cells.UnMerge(0, 0, 2, 2);

            // Güncellenmiş birleştirilmiş hücre sayısını ve aralıklarını göster
            Console.WriteLine($"\nAfter unmerging A1:B2 - Merged cells count: {cells.MergedCells.Count}");
            foreach (CellArea area in cells.MergedCells)
            {
                Console.WriteLine($"Remaining merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Sonucu kaydet
            workbook.Save("PropertyMergedCellsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


