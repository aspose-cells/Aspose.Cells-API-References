---
title: "PivotTable.ShowDetail"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. Veri bölgesindeki bir öğenin detayını yeni bir tabloya göster"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/showdetail/
---
## PivotTable.ShowDetail method

Veri bölgesindeki bir öğenin ayrıntısını yeni bir tabloya göster.

```csharp
public void ShowDetail(int rowOffset, int columnOffset, bool newSheet, int destRow, int destColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | Int32 | Veri bölgesindeki ilk veri satırına ofset |
| columnOffset | Int32 | Veri bölgesindeki ilk veri sütununa ofset |
| newSheet | Boolean | Detayı yeni bir çalışma sayfasına göster |
| destRow | Int32 | Hedef satır. |
| destColumn | Int32 | Hedef sütun. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowDetailWithInt32Int32BooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Sport");
            worksheet.Cells["A2"].PutValue("Tennis");
            worksheet.Cells["A3"].PutValue("Basketball");
            worksheet.Cells["A4"].PutValue("Tennis");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(80);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(85);

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Sport");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Score");

            // Belirli hücre için detayı göster
            pivotTable.ShowDetail(1, 0, true, 0, 0);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableShowDetailExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


