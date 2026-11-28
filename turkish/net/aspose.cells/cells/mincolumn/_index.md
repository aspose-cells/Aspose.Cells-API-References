---
title: "Cells.MinColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Koleksiyonda örneklenmiş olan hücrelerin minimum sütun indeksi, tüm sütun için stil tanımlı olduğu ancak hiçbir hücrenin örneklenmediği sütunu içermez."
type: docs
url: /tr/net/aspose.cells/cells/mincolumn/
---
## Cells.MinColumn property

Koleksiyonda oluşturulmuş hücrelerin minimum sütun indeksi (tüm sütun için stil tanımlı ancak içinde hücre oluşturulmamış sütunu içermez).

```csharp
public int MinColumn { get; }
```

### Açıklamalar

Bu özellik, hücreleri ve satırları dinamik olarak yinelemek ve kontrol etmek zorundadır, bu yüzden zaman tüketen bir işlemdir ve bir döngüde doğrudan koşul olarak kullanmak gibi tekrar tekrar çağrılmamalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Cells koleksiyonuna eriş
            Cells cells = worksheet.Cells;
            
            // 2, 3 ve 4. sütunlara (B, C, D) bazı veriler ekleyin.
            cells["B1"].PutValue("Data in Column B");
            cells["C1"].PutValue("Data in Column C");
            cells["D1"].PutValue("Data in Column D");
            
            // Veri içeren minimum sütun indeksini alın.
            int minColumn = cells.MinColumn;
            
            // Veri içeren maksimum sütun indeksini alın.
            int maxColumn = cells.MaxColumn;
            
            Console.WriteLine("Minimum column with data: " + minColumn); // Should output 1 (column B)
            Console.WriteLine("Maximum column with data: " + maxColumn); // Should output 3 (column D)
            
            // MinColumn değişikliğini göstermek için B sütununu temizleyin.
            cells.DeleteColumn(1);
            
            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("New minimum column with data: " + cells.MinColumn); // Should now output 2 (column C)
            Console.WriteLine("Maximum column with data: " + cells.MaxColumn); // Should still output 3 (column D)
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


