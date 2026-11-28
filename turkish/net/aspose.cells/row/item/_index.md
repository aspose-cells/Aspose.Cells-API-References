---
title: "Row.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Row özelliği. Hücreyi alır"
type: docs
url: /tr/net/aspose.cells/row/item/
---
## Row indexer

Hücreyi alır.

```csharp
public Cell this[int column] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| sütun | Sütun indeksi |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // İlk satıra eriş
            Row row = sheet.Cells.Rows[0];
            
            // Farklı renk stilleriyle HTML içeriği ayarla
            row[0].HtmlString = @"<span style=""color:#ffAb68;"">TEST</span>";
            row[1].HtmlString = @"<span style=""color:inherit;"">TEST</span>";
            
            // Item özelliğinin kullanımını göster ve renkleri çıktıya al
            Console.WriteLine("Cell 0 Font Color: " + row[0].GetStyle().Font.Color.Name);
            Console.WriteLine("Cell 1 Font Color: " + row[1].GetStyle().Font.Color.Name);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


