---
title: "Row.IsBlank"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Row özelliği. Satırın herhangi bir veri içerip içermediğini gösterir"
type: docs
url: /tr/net/aspose.cells/row/isblank/
---
## Row.IsBlank property

Satırın herhangi bir veri içerip içermediğini gösterir.

```csharp
public bool IsBlank { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsBlankDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk satırı al (başlangıçta boş)
            Row row1 = worksheet.Cells.Rows[0];
            Console.WriteLine("Row 1 IsBlank: " + row1.IsBlank); // True
            
            // İlk satıra veri ekle
            worksheet.Cells["A1"].PutValue("Test");
            Console.WriteLine("Row 1 IsBlank after adding data: " + row1.IsBlank); // False
            
            // Başka bir boş satır oluştur
            Row row2 = worksheet.Cells.Rows[1];
            Console.WriteLine("Row 2 IsBlank: " + row2.IsBlank); // True
            
            // Satırın boş durumunu karşılaştır
            Console.WriteLine("Rows have same IsBlank status: " + (row1.IsBlank == row2.IsBlank)); // False
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


