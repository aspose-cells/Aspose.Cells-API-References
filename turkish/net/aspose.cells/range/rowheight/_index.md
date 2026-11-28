---
title: "Range.RowHeight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Bu aralıktaki satırların yüksekliğini ayarlar veya alır"
type: docs
url: /tr/net/aspose.cells/range/rowheight/
---
## Range.RowHeight property

Bu aralıktaki satırların yüksekliğini ayarlar veya alır

```csharp
public double RowHeight { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowHeightDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk satıra bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("This is a test");
            worksheet.Cells["B1"].PutValue("to demonstrate");
            worksheet.Cells["C1"].PutValue("RowHeight property");

            // İlk satır yüksekliğini alın
            double initialHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Initial row height: " + initialHeight);

            // Satırı otomatik olarak sığdırın
            worksheet.AutoFitRow(0);

            // Otomatik sığdırmadan sonra yeni satır yüksekliğini alın
            double newHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Row height after auto-fit: " + newHeight);

            // Manuel olarak yeni bir satır yüksekliği ayarlayın
            worksheet.Cells.CreateRange("1:1").RowHeight = 30;
            Console.WriteLine("Row height after manual set: " + worksheet.Cells.CreateRange("1:1").RowHeight);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


