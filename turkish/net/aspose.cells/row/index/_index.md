---
title: "Row.Index"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Satır özelliği. Bu satırın indeksini alır"
type: docs
url: /tr/net/aspose.cells/row/index/
---
## Row.Index property

Bu satırın dizinini alır.

```csharp
public int Index { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIndexDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Satırlar arasında döngü yapın ve Index özelliğini gösterin
            foreach (Row row in worksheet.Cells.Rows)
            {
                Console.WriteLine($"Processing row with index: {row.Index}");
                if (row.Index > 0) // Skip header row
                {
                    Console.WriteLine($"Data in row {row.Index}: " +
                        $"{worksheet.Cells[row.Index, 0].StringValue}, " +
                        $"{worksheet.Cells[row.Index, 1].IntValue}");
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


