---
title: "Enum PivotConditionFormatScopeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotConditionFormatScopeType‑enum. Representerar pivottabellens villkorsformateringsomfångstyp"
type: docs
url: /sv/net/aspose.cells.pivot/pivotconditionformatscopetype/
---
## PivotConditionFormatScopeType enumeration

Representerar PivotTable‑villkorsformateringsomfångstyp.

```csharp
public enum PivotConditionFormatScopeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Data | `0` | Indikerar att villkorsformatering tillämpas på de markerade datafälten. |
| Field | `1` | Indikerar att villkorsformatering tillämpas på de markerade pivottabellens fältkorsningar. |
| Selection | `2` | Indikerar att villkorsformatering tillämpas på de markerade cellerna. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotConditionFormatScopeTypeDemo
    {
        public static void PivotConditionFormatScopeTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till lite data i kalkylbladet
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Lägg till en pivottabell
            PivotTableCollection pivots = worksheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Lägg till PivotFormatCondition
            int formatIndex = pivot.PivotFormatConditions.Add();
            PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
            FormatConditionCollection fcc = pfc.FormatConditions;
            fcc.AddArea(pivot.DataBodyRange);
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;

            // Ange omfångstypen för pivottabellens villkorsformat
            pfc.ScopeType = PivotConditionFormatScopeType.Data;

            pivot.RefreshData();
            pivot.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotConditionFormatScopeTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


