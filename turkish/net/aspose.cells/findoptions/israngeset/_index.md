---
title: "FindOptions.IsRangeSet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FindOptions özelliği. Aranan aralığın ayarlanıp ayarlanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/findoptions/israngeset/
---
## FindOptions.IsRangeSet property

Aranan aralığın ayarlanıp ayarlanmadığını gösterir.

```csharp
public bool IsRangeSet { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertyIsRangeSetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı verileri doldurun
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Date");
            worksheet.Cells["B2"].PutValue("Elderberry");
            worksheet.Cells["B3"].PutValue("Fig");

            // FindOptions örneği oluştur
            FindOptions findOptions = new FindOptions();

            // İlk IsRangeSet değerini kontrol edin (false olmalı)
            Console.WriteLine("Initial IsRangeSet value: " + findOptions.IsRangeSet);

            // Bir arama aralığı ayarlayın
            CellArea searchRange = new CellArea();
            searchRange.StartRow = 0;
            searchRange.StartColumn = 0;
            searchRange.EndRow = 2;
            searchRange.EndColumn = 0; // Column A only
            findOptions.SetRange(searchRange);

            // Aralık ayarlandıktan sonra IsRangeSet'i kontrol edin (true olmalı)
            Console.WriteLine("After SetRange, IsRangeSet value: " + findOptions.IsRangeSet);

            // Belirtilen aralık içinde bir bulma işlemi gerçekleştirin
            Cell foundCell = worksheet.Cells.Find("Banana", null, findOptions);
            Console.WriteLine("Found 'Banana' at: " + foundCell?.Name);

            // Aralık dışındaki bir şeyi bulmayı deneyin (bulunmamalı)
            foundCell = worksheet.Cells.Find("Fig", null, findOptions);
            Console.WriteLine("Found 'Fig' at: " + foundCell?.Name); // Should be null

            // Çalışma kitabını kaydedin
            workbook.Save("PropertyIsRangeSetDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


