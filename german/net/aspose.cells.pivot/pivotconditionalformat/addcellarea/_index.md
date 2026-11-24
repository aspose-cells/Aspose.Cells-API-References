---
title: "PivotConditionalFormat.AddCellArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotConditionalFormat-Methode. Fügt einen Bereich basierend auf der Pivot-Tabellenansicht hinzu"
type: docs
url: /de/net/aspose.cells.pivot/pivotconditionalformat/addcellarea/
---
## PivotConditionalFormat.AddCellArea method

Fügt einen Bereich basierend auf der Pivot‑Tabellenansicht hinzu.

```csharp
public void AddCellArea(CellArea ca)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | CellArea | Der Zellbereich. |

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 120;
            cells["B3"].Value = 85;
            cells["B4"].Value = 90;

            // PivotTable hinzufügen
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Erstellen Sie einen Zellbereich für die bedingte Formatierung
            CellArea cellArea = new CellArea();
            cellArea.StartRow = 4;
            cellArea.StartColumn = 5;
            cellArea.EndRow = 6;
            cellArea.EndColumn = 7;

            // Fügen Sie ein bedingtes Format mit Zellbereich hinzu
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
            pcf.AddCellArea(cellArea);

            // Formatbedingung hinzufügen
            int conditionIndex = pcf.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pcf.FormatConditions[conditionIndex];
            condition.Formula1 = "50";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.LightGreen;

            // PivotTable-Daten berechnen
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotConditionalFormatWithCellArea.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


