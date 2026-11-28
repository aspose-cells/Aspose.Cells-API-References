---
title: "Cells.Rows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Bu çalışma sayfasındaki bireysel satırları temsil eden Row nesnelerinin koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/cells/rows/
---
## Cells.Rows property

Bu çalışma sayfasındaki bireysel satırları temsil eden [`Row`](../../row/) nesnelerinin koleksiyonunu alır.

```csharp
public RowCollection Rows { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRowsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sütun genişliğini ve satır yüksekliğini ayarlayın
            worksheet.Cells.SetColumnWidthPixel(0, 200);
            worksheet.Cells.Rows[0].Height = 50;
            
            // Rows koleksiyonu aracılığıyla satır özelliklerine erişin
            Row row = worksheet.Cells.Rows[0];
            Console.WriteLine($"Row 0 height: {row.Height}");
            Console.WriteLine($"Is height matched: {row.IsHeightMatched}");
            
            // Satır özelliklerini değiştirin
            row.IsHeightMatched = true;
            row.Height = 60;
            
            // Değişiklikleri doğrula
            Console.WriteLine($"Modified row 0 height: {worksheet.Cells.GetRowHeightPixel(0)}");
            Console.WriteLine($"Is height matched after change: {row.IsHeightMatched}");
            
            // Çalışma kitabını kaydedin
            workbook.Save("CellsPropertyRowsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [RowCollection](../../rowcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


