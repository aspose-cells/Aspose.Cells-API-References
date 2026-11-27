---
title: "PivotArea.AxisType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotArea-egenskap. Hämtar och anger regionen i pivottabellen som denna regel gäller för"
type: docs
url: /sv/net/aspose.cells.pivot/pivotarea/axistype/
---
## PivotArea.AxisType property

Hämtar och anger regionen för pivottabellen som denna regel gäller för.

```csharp
public PivotFieldType AxisType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyAxisTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 800;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivotområden
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Sales

            // Skapa och konfigurera PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row; // Demonstrate AxisType property
            pivotArea.RuleType = PivotAreaType.Normal;

            // Välj pivotområdet
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Spara arbetsboken
            workbook.Save("PivotAreaAxisTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


