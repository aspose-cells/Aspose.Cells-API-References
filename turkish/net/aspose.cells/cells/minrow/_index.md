---
title: "Cells.MinRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Veri veya stil içeren hücrenin minimum satır indeksi"
type: docs
url: /tr/net/aspose.cells/cells/minrow/
---
## Cells.MinRow property

Veri veya stil içeren hücrenin minimum satır indeksi.

```csharp
public int MinRow { get; }
```

### Açıklamalar

Bu özellik, hücreleri ve satırları dinamik olarak yinelemek ve kontrol etmek zorundadır, bu yüzden zaman tüketen bir işlemdir ve bir döngüde doğrudan koşul olarak kullanmak gibi tekrar tekrar çağrılmamalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // MinRow'u göstermek için bazı veriler ekleyin
            cells["A1"].PutValue("Data in first row");
            cells["B5"].PutValue("Data in fifth row");

            // MinRow bilgilerini göster
            Console.WriteLine("Minimum used row: " + cells.MinRow);
            Console.WriteLine("Maximum used row: " + cells.MaxRow);

            // MinRow'dan itibaren içeriği temizle
            cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);

            // Hücrelerin boş olup olmadığını kontrol ederek temizlemeyi doğrulayın
            Console.WriteLine("A1 after clearing: " + (cells["A1"].Value == null ? "Empty" : "Not empty"));
            Console.WriteLine("B5 after clearing: " + (cells["B5"].Value == null ? "Empty" : "Not empty"));
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


