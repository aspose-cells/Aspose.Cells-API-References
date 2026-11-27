---
title: "PivotTable.ConditionalFormats"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar de villkorliga formaten för pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/conditionalformats/
---
## PivotTable.ConditionalFormats property

Hämtar de villkorsformat som används i pivottabellen.

```csharp
public PivotConditionalFormatCollection ConditionalFormats { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyConditionalFormatsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 120;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 85;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 95;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 110;

            // Skapa pivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Lägg till rad- och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Lägg till villkorligt format
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.AddFieldArea(PivotFieldType.Data, pivotTable.DataFields[0]);
            
            // Lägg till formatvillkor
            int conditionIndex = pcf.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pcf.FormatConditions[conditionIndex];
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Formula1 = "100";
            condition.Style.BackgroundColor = Color.Red;

            // Spara arbetsbok
            workbook.Save("PivotTableConditionalFormatting.xlsx");
        }
    }
}
```

### Se även

* class [PivotConditionalFormatCollection](../../pivotconditionalformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


