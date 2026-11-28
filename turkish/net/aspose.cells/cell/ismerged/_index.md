---
title: "Cell.IsMerged"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Bir hücrenin birleştirilmiş bir aralığın parçası olup olmadığını kontrol eder"
type: docs
url: /tr/net/aspose.cells/cell/ismerged/
---
## Cell.IsMerged property

Bir hücrenin birleştirilmiş bir aralığın parçası olup olmadığını kontrol eder.

```csharp
public bool IsMerged { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsMergedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1'den B2'ye hücreleri birleştirin
            worksheet.Cells.Merge(0, 0, 2, 2);

            // A1 hücresinin birleştirilip birleştirilmediğini kontrol edin
            bool isMerged = worksheet.Cells["A1"].IsMerged;
            Console.WriteLine("Is cell A1 merged? " + isMerged);

            // C1 hücresinin birleştirilip birleştirilmediğini kontrol edin (false olmalı)
            isMerged = worksheet.Cells["C1"].IsMerged;
            Console.WriteLine("Is cell C1 merged? " + isMerged);

            // Çalışma kitabını kaydedin
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


