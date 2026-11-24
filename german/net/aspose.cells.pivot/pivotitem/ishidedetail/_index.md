---
title: "PivotItem.IsHideDetail"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotItem-Eigenschaft. Gibt an und legt fest, ob das Pivot-Element Details ausblendet"
type: docs
url: /de/net/aspose.cells.pivot/pivotitem/ishidedetail/
---
## PivotItem.IsHideDetail property

Gibt an und legt fest, ob das Pivot-Element Details ausblendet.

```csharp
[Obsolete("Use PivotItem.IsDetailHidden property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHideDetail { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft PivotItem.IsDetailHidden. Diese Eigenschaft wird 12 Monate nach November 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsHideDetailDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            foreach (PivotItem pivotItem in pivotItems)
            {
                Console.WriteLine($"Original IsHideDetail: {pivotItem.IsHideDetail}");
                pivotItem.IsHideDetail = true;
                Console.WriteLine($"Modified IsHideDetail: {pivotItem.IsHideDetail}");
            }

            workbook.Save("PivotItemIsHideDetailDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


