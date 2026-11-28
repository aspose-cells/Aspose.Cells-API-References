---
title: "Cells.MaxRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Veri veya stil içeren hücrenin maksimum satır indeksi"
type: docs
url: /tr/net/aspose.cells/cells/maxrow/
---
## Cells.MaxRow property

Veri veya stil içeren hücrenin maksimum satır indeksi.

```csharp
public int MaxRow { get; }
```

### Açıklamalar

Çalışma sayfasında veri veya stil içeren hücre yoksa -1 döndür. Bu özellik, hücreleri ve satırları dinamik olarak yinelemek ve kontrol etmek zorunda olduğundan zaman tüketen bir işlemdir ve bir döngüde doğrudan koşul olarak kullanmak gibi tekrar tekrar çağrılmamalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek veri ekleyin
            cells[0, 0].PutValue("Name");
            cells[0, 1].PutValue("Age");
            cells[1, 0].PutValue("John");
            cells[1, 1].PutValue(30);
            cells[2, 0].PutValue("Alice");
            cells[2, 1].PutValue(25);

            // Maksimum satır indeksini al (sıfır tabanlı)
            int maxRow = cells.MaxRow;
            Console.WriteLine("MaxRow before adding new data: " + maxRow);

            // Maksimum satırın ardından sonraki satıra yeni veri ekle
            int newRow = maxRow + 1;
            cells[newRow, 0].PutValue("Bob");
            cells[newRow, 1].PutValue(28);

            // Yeni maksimum satırı doğrula
            Console.WriteLine("MaxRow after adding new data: " + cells.MaxRow);

            // Çalışma kitabını kaydedin
            workbook.Save("MaxRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


