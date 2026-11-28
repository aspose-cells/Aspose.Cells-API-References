---
title: "FindOptions.SearchOrderByRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FindOptions özelliği. Arama sırasının satır mı sütun mu olduğunu gösterir"
type: docs
url: /tr/net/aspose.cells/findoptions/searchorderbyrows/
---
## FindOptions.SearchOrderByRows property

Arama sırasının satır mı yoksa sütun mu olduğunu gösterir.

```csharp
public bool SearchOrderByRows { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchOrderByRowsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve örnek veri ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücreleri test verileriyle doldurun (\"abc\"yi sütun‑öncelikli sırada arayarak)
            worksheet.Cells["A1"].PutValue("xyz");
            worksheet.Cells["B1"].PutValue("def");
            worksheet.Cells["A2"].PutValue("123");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("abc");
            worksheet.Cells["B3"].PutValue("789");

            // FindOptions oluşturun ve arama sırasını sütun‑öncelikli olarak ayarlayın
            FindOptions findOptions = new FindOptions();
            findOptions.SearchOrderByRows = false; // Search column by column

            // \"abc\"yi bulun - sütun‑öncelikli arama yapıldığında A3 (satır 2, sütun 0) döndürmelidir
            Cell foundCell = worksheet.Cells.Find("abc", null, findOptions);

            // Sonucu çıktı olarak ver
            Console.WriteLine($"Found 'abc' at row: {foundCell.Row}, column: {foundCell.Column}");
        }
    }
}
```

### Ayrıca Bakınız

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


