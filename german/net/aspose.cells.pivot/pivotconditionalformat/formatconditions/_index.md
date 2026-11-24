---
title: "PivotConditionalFormat.FormatConditions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotConditionalFormat-Eigenschaft. Bedingungen für das Pivot-Tabellen-Bedingungsformat abrufen"
type: docs
url: /de/net/aspose.cells.pivot/pivotconditionalformat/formatconditions/
---
## PivotConditionalFormat.FormatConditions property

Lese Bedingungen für das bedingte Format der Pivot‑Tabelle.

```csharp
public FormatConditionCollection FormatConditions { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatPropertyFormatConditionsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 120;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 85;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 95;

            // PivotTable hinzufügen
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Bedingtes Format hinzufügen
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 1;
            area.EndRow = 3;
            area.EndColumn = 1;
            pfc.AddCellArea(area); // Apply to quantity column

            // Formatbedingung hinzufügen
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = pfc.FormatConditions[conditionIndex];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = System.Drawing.Color.Red;

            // PivotTable-Daten berechnen
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotConditionalFormatExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatConditionCollection](../../../aspose.cells/formatconditioncollection/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


