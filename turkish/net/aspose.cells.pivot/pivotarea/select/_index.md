---
title: "PivotArea.Select"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotArea yöntemi. Filtrelerle alanı seçin"
type: docs
url: /tr/net/aspose.cells.pivot/pivotarea/select/
---
## PivotArea.Select method

Filtrelerle alanı seç.

```csharp
public void Select(PivotFieldType axisType, int fieldPosition, 
    PivotTableSelectionType selectionType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| axisType | PivotFieldType | Bu kuralın uygulandığı PivotTable bölgesi. |
| fieldPosition | Int32 | Bu kuralın uygulandığı eksen içindeki alanın konumu. |
| selectionType | PivotTableSelectionType | Yapılandırılmış bir seçim sırasında bir PivotTable'da neyin seçilebileceğini belirtir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodSelectWithPivotFieldTypeInt32PivotTableSDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            workbook.Save("PivotAreaSelectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


