---
title: "FindOptions.ValueTypeSensitive"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FindOptions özelliği. Aranan hücre değer tipinin aranan anahtar ile aynı olması gerekip gerekmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/findoptions/valuetypesensitive/
---
## FindOptions.ValueTypeSensitive property

Aranan hücre değer tipinin aranan anahtar ile aynı olması gerekip gerekmediğini gösterir.

```csharp
public bool ValueTypeSensitive { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyValueTypeSensitiveDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve örnek veri ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere farklı değer tipleri ekleyin
            worksheet.Cells["A1"].PutValue("100"); // Stored as string
            worksheet.Cells["A2"].PutValue(100);   // Stored as number
            worksheet.Cells["A3"].PutValue("100.0"); // Stored as string
            worksheet.Cells["A4"].PutValue(100.0);   // Stored as number

            // FindOptions oluşturun ve ValueTypeSensitive = true ayarlayın
            FindOptions options = new FindOptions();
            options.ValueTypeSensitive = true;
            options.LookAtType = LookAtType.EntireContent;

            // 100 sayısını ara (\"100\" dizesini bulamaz)
            Cell foundCell = worksheet.Cells.Find(100, null, options);
            Console.WriteLine("Found cell with number 100: " + (foundCell != null ? foundCell.Name : "Not found"));

            // \"100\" dizesini ara (100 sayısını bulamaz)
            foundCell = worksheet.Cells.Find("100", null, options);
            Console.WriteLine("Found cell with string \"100\": " + (foundCell != null ? foundCell.Name : "Not found"));

            // ValueTypeSensitive = false olarak değiştirin
            options.ValueTypeSensitive = false;
            
            // Artık her iki arama da \"100\" veya 100 içeren herhangi bir hücreyi bulacaktır
            foundCell = worksheet.Cells.Find(100, null, options);
            Console.WriteLine("Found any 100 (type insensitive): " + (foundCell != null ? foundCell.Name : "Not found"));
        }
    }
}
```

### Ayrıca Bakınız

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


