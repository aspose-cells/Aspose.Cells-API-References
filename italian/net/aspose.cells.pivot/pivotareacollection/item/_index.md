---
title: "PivotAreaCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotAreaCollection. Restituisce un oggetto PivotArea"
type: docs
url: /it/net/aspose.cells.pivot/pivotareacollection/item/
---
## PivotAreaCollection indexer

Restituisce un oggetto [`PivotArea`](../../pivotarea/);

```csharp
public PivotArea this[int index] { get; }
```

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 150;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 200;

            // Crea tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A5", "A1:B4", "PivotTable");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi formato condizionale
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            pfc.AddCellArea(CellArea.CreateCellArea("A5", "B8"));

            // Accedi a PivotAreas usando la proprietà Item
            PivotArea pivotArea = pfc.PivotAreas[0]; // Using Item indexer
            pivotArea.RuleType = PivotAreaType.All;

            // Aggiungi condizione di formato
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "150";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = Color.Red;

            // Calcola e salva
            pivot.CalculateData();
            workbook.Save("PivotAreaCollectionPropertyItemDemo_output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotArea](../../pivotarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


