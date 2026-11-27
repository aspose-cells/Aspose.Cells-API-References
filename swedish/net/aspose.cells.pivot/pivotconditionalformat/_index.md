---
title: "Class PivotConditionalFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotConditionalFormat class. Representerar det villkorliga formatet för pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivotconditionalformat/
---
## PivotConditionalFormat class

Representerar det villkorliga formatet för pivottabellen.

```csharp
public class PivotConditionalFormat
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FormatConditions](../../aspose.cells.pivot/pivotconditionalformat/formatconditions/) { get; } | Hämta villkor för pivottabellens villkorliga format. |
| [PivotAreas](../../aspose.cells.pivot/pivotconditionalformat/pivotareas/) { get; } | Hämtar alla pivotområden. |
| [RuleType](../../aspose.cells.pivot/pivotconditionalformat/ruletype/) { get; set; } | Hämta och ange regeltyp för pivottabellens villkorliga format. |
| [ScopeType](../../aspose.cells.pivot/pivotconditionalformat/scopetype/) { get; set; } | Hämta och ange omfångstyp för pivottabellens villkorliga format. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddCellArea](../../aspose.cells.pivot/pivotconditionalformat/addcellarea/)(CellArea) | Lägger till ett område baserat på pivottabellvyn. |
| [AddFieldArea](../../aspose.cells.pivot/pivotconditionalformat/addfieldarea/#addfieldarea)(PivotFieldType, PivotField) | Lägger till ett område av pivottfältet. |
| [AddFieldArea](../../aspose.cells.pivot/pivotconditionalformat/addfieldarea/#addfieldarea_1)(PivotFieldType, string) | Lägger till ett område av pivottfältet. |
| [ApplyTo](../../aspose.cells.pivot/pivotconditionalformat/applyto/)(int, int, PivotConditionFormatScopeType) | Tillämpar det villkorliga formatet på ett område som måste vara i dataregionen. |
| [GetCellAreas](../../aspose.cells.pivot/pivotconditionalformat/getcellareas/)() | Hämtar alla cellområden där detta villkorliga format gäller. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotClassPivotConditionalFormatDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Ange exempeldata
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";
            
            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;
            
            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;
            
            // Skapa pivottabell
            int pivotIndex = sheet.PivotTables.Add("=A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            
            // Lägg till villkorsstyrd formatering
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            pfc.AddFieldArea(PivotFieldType.Data, pivot.DataFields[0]);
            
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = pfc.FormatConditions[conditionIndex];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;
            
            pivot.RefreshData();
            book.Save("PivotConditionalFormatDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


