---
title: "Column.Index"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Column özelliği. Bu sütunun indeksini alır"
type: docs
url: /tr/net/aspose.cells/column/index/
---
## Column.Index property

Bu sütunun dizinini alır.

```csharp
public int Index { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIndexDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sütunlara bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            
            // Sütun koleksiyonunu al
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Index özelliğini göster
            Console.WriteLine("Column Indices:");
            for (int i = 0; i < columns.Count; i++)
            {
                Column column = columns[i];
                Console.WriteLine($"Column {column.Index}: {worksheet.Cells[0, column.Index].StringValue}");
            }
            
            // Sütuna indeks ile eriş
            Column columnB = columns[1]; // B column (index 1)
            Console.WriteLine($"\nAccessed by index 1: {worksheet.Cells[0, columnB.Index].StringValue}");
            
            // İndeks kullanarak sütun genişliğini değiştir
            columns[2].Width = 30; // C column (index 2)
            Console.WriteLine($"\nColumn C width set to: {columns[2].Width}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


