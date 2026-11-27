---
title: "PivotAreaCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotAreaCollection-egenskap. Hämtar ett PivotArea-objekt."
type: docs
url: /sv/net/aspose.cells.pivot/pivotareacollection/item/
---
## PivotAreaCollection indexer

Hämtar ett [`PivotArea`](../../pivotarea/) objekt;

```csharp
public PivotArea this[int index] { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotAreaCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 150;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 200;

            // Skapa pivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A5", "A1:B4", "PivotTable");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Lägg till villkorligt format
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            pfc.AddCellArea(CellArea.CreateCellArea("A5", "B8"));

            // Åtkomst till PivotAreas via Item-egenskapen.
            PivotArea pivotArea = pfc.PivotAreas[0]; // Using Item indexer
            pivotArea.RuleType = PivotAreaType.All;

            // Lägg till formatvillkor
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "150";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = Color.Red;

            // Beräkna och spara
            pivot.CalculateData();
            workbook.Save("PivotAreaCollectionPropertyItemDemo_output.xlsx");
        }
    }
}
```

### Se även

* class [PivotArea](../../pivotarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


