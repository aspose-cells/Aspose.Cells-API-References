---
title: "Range.FirstRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Aralığın ilk satırının indeksini alır"
type: docs
url: /tr/net/aspose.cells/range/firstrow/
---
## Range.FirstRow property

Aralığın ilk satırının indeksini alır.

```csharp
public int FirstRow { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve ilk worksheet'e erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı verileri doldurun
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Bir aralık oluşturun
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // FirstRow özelliğine erişin ve görüntüleyin
            Console.WriteLine("First row index of range: " + range.FirstRow);

            // Aralığın ilk satırındaki ilk hücreye erişin
            Cell firstCell = worksheet.Cells[range.FirstRow, range.FirstColumn];
            Console.WriteLine("First cell value: " + firstCell.StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


