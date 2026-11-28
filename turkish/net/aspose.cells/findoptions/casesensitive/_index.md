---
title: "FindOptions.CaseSensitive"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FindOptions özelliği. Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/findoptions/casesensitive/
---
## FindOptions.CaseSensitive property

Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir.

```csharp
public bool CaseSensitive { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veriyi ayarla
            worksheet.Cells["A1"].PutValue("ABC");
            worksheet.Cells["A2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("BcD");

            FindOptions options = new FindOptions();
            options.CaseSensitive = true;
            
            // \"bc\"yi büyük/küçük harfe duyarlılık ile ara
            Cell cell = worksheet.Cells.Find("bc", null, options);
            
            Console.WriteLine(cell == null ? "Not found (case sensitive)" : $"Found at: {cell.Name}");
            
            options.CaseSensitive = false;
            cell = worksheet.Cells.Find("bc", null, options);
            
            Console.WriteLine(cell == null ? "Not found" : $"Found at: {cell.Name}");
        }
    }
}
```

### Ayrıca Bakınız

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


