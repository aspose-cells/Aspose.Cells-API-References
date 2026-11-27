---
title: "PivotConditionalFormat.AddCellArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotConditionalFormat-metod. Lägger till ett område baserat på pivottabellvyn"
type: docs
url: /sv/net/aspose.cells.pivot/pivotconditionalformat/addcellarea/
---
## PivotConditionalFormat.AddCellArea method

Lägger till ett område baserat på pivottabellvyn.

```csharp
public void AddCellArea(CellArea ca)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | CellArea | Cellområdet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodAddCellAreaWithCellAreaDemo
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
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 120;
            cells["B3"].Value = 85;
            cells["B4"].Value = 90;

            // Lägg till pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Skapa ett cellområde för villkorsformatering
            CellArea cellArea = new CellArea();
            cellArea.StartRow = 4;
            cellArea.StartColumn = 5;
            cellArea.EndRow = 6;
            cellArea.EndColumn = 7;

            // Lägg till villkorsformat med cellområde
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.AddCellArea(cellArea);

            // Lägg till formatvillkor
            int conditionIndex = pcf.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pcf.FormatConditions[conditionIndex];
            condition.Formula1 = "50";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.LightGreen;

            // Beräkna pivottabellsdata
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotConditionalFormatWithCellArea.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


