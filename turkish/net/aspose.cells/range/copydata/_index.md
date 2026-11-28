---
title: "Range.CopyData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Kaynak bir aralıktan formüller dahil hücre verilerini kopyalar"
type: docs
url: /tr/net/aspose.cells/range/copydata/
---
## Range.CopyData method

Kaynak bir aralıktan hücre verisini (formüller dahil) kopyalar.

```csharp
public void CopyData(Range range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| range | Range | Kaynak [`Range`](../) nesnesi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyDataWithRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasını al ve bazı veri ekle
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            sheetSrc.Cells["A1"].PutValue("Source Data");
            sheetSrc.Cells["B1"].PutValue(100);
            sheetSrc.Cells["A2"].PutValue("More Data");
            sheetSrc.Cells["B2"].PutValue(200);

            // Bir hedef çalışma sayfası ekle
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";

            // Kaynak ve hedef aralıklar oluştur
            Aspose.Cells.Range rangeSrc = sheetSrc.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("C3:D4");

            // Verileri kaynak aralıktan hedef aralığa kopyala
            rangeDest.CopyData(rangeSrc);

            // Çalışma kitabını kaydedin
            workbook.Save("RangeCopyDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


