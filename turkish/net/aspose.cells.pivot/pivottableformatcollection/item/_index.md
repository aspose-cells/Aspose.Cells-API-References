---
title: "PivotTableFormatCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTableFormatCollection özelliği. Formatı indeksle alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivottableformatcollection/item/
---
## PivotTableFormatCollection indexer

Formatı indeksine göre alır.

```csharp
public PivotTableFormat this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");

            // Tüm pivot tabloları yenile
            workbook.Worksheets.RefreshAll();
            Cells cells = workbook.Worksheets[0].Cells;

            // İlk pivot tabloya eriş
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];

            // İlk PivotFormat'a erişerek Item özelliğini göster
            pt.PivotFormats[0].PivotArea.OnlyData = false;
            workbook.Worksheets.RefreshAll();

            // Item özelliğini kullanarak biçim ayarlarını değiştirin
            pt.PivotFormats[0].PivotArea.OnlyLabel = true;
            workbook.Worksheets.RefreshAll();

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("modified_example.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableFormat](../../pivottableformat/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


