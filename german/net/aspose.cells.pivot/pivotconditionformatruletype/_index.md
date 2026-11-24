---
title: "Aufzählung PivotConditionFormatRuleType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotConditionFormatRuleType enum. Stellt den Regeltyp für die bedingte Formatierung einer PivotTable dar"
type: docs
url: /de/net/aspose.cells.pivot/pivotconditionformatruletype/
---
## PivotConditionFormatRuleType enumeration

Stellt den Regeltyp für die bedingte Formatierung der PivotTable dar.

```csharp
public enum PivotConditionFormatRuleType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Gibt an, dass die Top‑N‑bedingte Formatierung nicht ausgewertet wird |
| All | `1` | Gibt an, dass die Top‑N‑bedingte Formatierung über den gesamten Geltungsbereich ausgewertet wird. |
| Row | `2` | Gibt an, dass die Top‑N‑bedingte Formatierung für jede Zeile ausgewertet wird. |
| Column | `3` | Gibt an, dass die Top‑N‑bedingte Formatierung für jede Spalte ausgewertet wird. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotConditionFormatRuleTypeDemo
    {
        public static void PivotConditionFormatRuleTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fügen Sie einige Beispieldaten hinzu
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

            // Fügen Sie eine Pivot-Tabelle hinzu
            PivotTableCollection pivots = worksheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Füge PivotFormatCondition hinzu
            int formatIndex = pivot.PivotFormatConditions.Add();
            PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
            FormatConditionCollection fcc = pfc.FormatConditions;
            fcc.AddArea(pivot.DataBodyRange);
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;

            // Setzen Sie den Regeltyp für die bedingte Formatierung der PivotTable fest.
            pfc.RuleType = PivotConditionFormatRuleType.Row;

            // Aktualisieren und berechnen Sie die Pivot-Tabellendaten
            pivot.RefreshData();
            pivot.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotConditionFormatRuleTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


