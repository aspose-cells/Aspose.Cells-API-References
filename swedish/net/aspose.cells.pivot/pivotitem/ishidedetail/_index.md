---
title: "PivotItem.IsHideDetail"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem-egenskap. Hämtar och anger om pivotobjektet döljer detaljer"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/ishidedetail/
---
## PivotItem.IsHideDetail property

Hämtar och anger om pivotobjektet döljer detaljer.

```csharp
[Obsolete("Use PivotItem.IsDetailHidden property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHideDetail { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotItem.IsDetailHidden-egenskapen. Denna egenskap kommer att tas bort 12 månader senare sedan november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


