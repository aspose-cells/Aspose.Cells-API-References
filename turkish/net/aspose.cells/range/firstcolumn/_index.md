---
title: "Range.FirstColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Aralığın ilk sütununun indeksini alır"
type: docs
url: /tr/net/aspose.cells/range/firstcolumn/
---
## Range.FirstColumn property

Aralığın ilk sütununun indeksini alır.

```csharp
public int FirstColumn { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri oluştur
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Bir aralık oluşturun
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");

            // FirstColumn özelliğini göster
            Console.WriteLine("First column index of range: " + range.FirstColumn);

            // FirstColumn'ı kullanarak aralığın ilk sütunundaki hücrelere eriş
            for (int i = 0; i < range.RowCount; i++)
            {
                Cell cell = range[i, 0]; // Access first column (index 0) of the range
                Console.WriteLine($"Cell[{i},0] value: {cell.StringValue}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("RangeFirstColumnDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


