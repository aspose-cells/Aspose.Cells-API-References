---
title: "Cell.GetMergedRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Birleştirilmiş aralığı temsil eden bir Range nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells/cell/getmergedrange/
---
## Cell.GetMergedRange method

Birleştirilmiş aralığı temsil eden bir [`Range`](../../range/) nesnesi döndürür.

```csharp
public Range GetMergedRange()
```

### Dönüş Değeri

[`Range`](../../range/) object. Null if this cell is not merged.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetMergedRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücreleri birleştir
            cells.Merge(0, 0, 2, 2);

            // İlk hücreyi al
            Cell cell = cells[0, 0];

            // Birleştirilmiş aralık bilgilerini al
            Aspose.Cells.Range mergedRange = cell.GetMergedRange();
            
            // Birleştirilmiş aralık ayrıntılarını çıktıla
            Console.WriteLine("Merged Range Details:");
            Console.WriteLine($"First Row: {mergedRange.FirstRow}");
            Console.WriteLine($"First Column: {mergedRange.FirstColumn}");
            Console.WriteLine($"Row Count: {mergedRange.RowCount}");
            Console.WriteLine($"Column Count: {mergedRange.ColumnCount}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


