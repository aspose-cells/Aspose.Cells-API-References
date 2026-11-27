---
title: "PivotConditionalFormat.ScopeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotConditionalFormat-egenskap. Hämta och ange omfångstyp för pivottabellens villkorsformat"
type: docs
url: /sv/net/aspose.cells.pivot/pivotconditionalformat/scopetype/
---
## PivotConditionalFormat.ScopeType property

Hämta och ange omfångstyp för pivottabellens villkorliga format.

```csharp
public PivotConditionFormatScopeType ScopeType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatPropertyScopeTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med en pivottabell
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Exempeldatat för pivottabell
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(300);

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Lägg till villkorsformat i pivottabellen
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.ScopeType = PivotConditionFormatScopeType.Data;

            // Lägg till formatvillkor
            FormatConditionCollection fcs = pcf.FormatConditions;
            CellArea area = new CellArea();
            area.StartRow = 4;
            area.EndRow = 6;
            area.StartColumn = 5;
            area.EndColumn = 5;
            int[] conditionIndex = fcs.Add(area, FormatConditionType.CellValue, OperatorType.Between, "100", "200");
            
            // Ange formatstil
            FormatCondition fc = fcs[conditionIndex[0]];
            fc.Style.BackgroundColor = Color.Yellow;

            // Spara arbetsboken
            wb.Save("PivotConditionalFormatScopeTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


