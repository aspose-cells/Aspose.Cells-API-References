---
title: "Cells.Ranges"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Çalışma zamanında oluşturulan Range nesnelerinin koleksiyonunu alır."
type: docs
url: /tr/net/aspose.cells/cells/ranges/
---
## Cells.Ranges property

Çalışma zamanında oluşturulan [`Range`](../../range/) nesnelerinin koleksiyonunu alır.

```csharp
public RangeCollection Ranges { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRangesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ranges koleksiyonuna bir aralık oluşturun ve ekleyin.
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Satırları ekleyin ve aralığın genişlediğini gösterin.
            worksheet.Cells.InsertRows(2, 2, true);
            
            Console.WriteLine($"Range row count after insertion: {cellRange.RowCount}");
        }
    }
}
```

### Ayrıca Bakınız

* class [RangeCollection](../../rangecollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


