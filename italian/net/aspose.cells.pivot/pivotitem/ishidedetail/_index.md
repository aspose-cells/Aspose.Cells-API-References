---
title: "PivotItem.IsHideDetail"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotItem. Ottiene e imposta se l'elemento pivot nasconde i dettagli"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/ishidedetail/
---
## PivotItem.IsHideDetail property

Ottiene e imposta se l'elemento pivot nasconde i dettagli.

```csharp
[Obsolete("Use PivotItem.IsDetailHidden property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHideDetail { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotItem.IsDetailHidden. Questa proprietà sarà rimossa 12 mesi dopo, a partire da novembre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

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

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


