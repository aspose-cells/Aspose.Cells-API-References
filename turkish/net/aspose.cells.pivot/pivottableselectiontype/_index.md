---
title: "Enum PivotTableSelectionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotTableSelectionType enum. Yapılandırılmış bir seçim sırasında bir PivotTable'da neyin seçilebileceğini belirtir. Bu sabitler birden fazla türü seçmek için birleştirilebilir."
type: docs
url: /tr/net/aspose.cells.pivot/pivottableselectiontype/
---
## PivotTableSelectionType enumeration

Yapılandırılmış bir seçim sırasında bir PivotTable'da neyin seçilebileceğini belirtir. Bu sabitler birden fazla türü seçmek için birleştirilebilir.

```csharp
public enum PivotTableSelectionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DataAndLabel | `0` | Veri ve etiketler |
| DataOnly | `2` | Yalnızca verileri seçer |
| LabelOnly | `1` | Yalnızca etiketleri seçer |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableSelectionTypeDemo
    {
        public static void PivotTableSelectionTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PivotTable için bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(250);

            // Bir PivotTable oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // PivotTable'a alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Bir PivotArea oluştur ve özelliklerini ayarla
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyData = false;
            pivotArea.OnlyLabel = true;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.IsOutline = false;

            // Belirli seçim türüyle alanı seç
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableSelectionTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


