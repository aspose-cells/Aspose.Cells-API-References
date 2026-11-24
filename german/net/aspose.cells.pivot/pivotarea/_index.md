---
title: "Klasse PivotArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotArea Klasse. Stellt den ausgewählten Bereich der PivotTable dar"
type: docs
url: /de/net/aspose.cells.pivot/pivotarea/
---
## PivotArea class

Stellt den ausgewählten Bereich der Pivot-Tabelle dar.

```csharp
public class PivotArea
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PivotArea](pivotarea/)(PivotTable) | Stellt den ausgewählten Bereich der PivotTable dar. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AxisType](../../aspose.cells.pivot/pivotarea/axistype/) { get; set; } | Liest und setzt den Bereich der PivotTable, für den diese Regel gilt. |
| [Filters](../../aspose.cells.pivot/pivotarea/filters/) { get; } | Liest alle Filter für diesen PivotArea. |
| [IsColumnGrandIncluded](../../aspose.cells.pivot/pivotarea/iscolumngrandincluded/) { get; set; } | Gibt an, ob die Gesamtsumme der Spalte enthalten ist. |
| [IsOutline](../../aspose.cells.pivot/pivotarea/isoutline/) { get; set; } | Gibt an, ob sich die Regel auf einen Bereich im Gliederungsmodus bezieht. |
| [IsRowGrandIncluded](../../aspose.cells.pivot/pivotarea/isrowgrandincluded/) { get; set; } | Gibt an, ob die Gesamtsumme der Zeile enthalten ist. |
| [OnlyData](../../aspose.cells.pivot/pivotarea/onlydata/) { get; set; } | Gibt an, ob nur die Datenwerte (im Datenbereich der Ansicht) für eine Elementauswahl ausgewählt sind und die Elementbeschriftungen nicht enthalten. |
| [OnlyLabel](../../aspose.cells.pivot/pivotarea/onlylabel/) { get; set; } | Gibt an, ob nur die Datenbeschriftungen für eine Elementauswahl ausgewählt sind. |
| [RuleType](../../aspose.cells.pivot/pivotarea/ruletype/) { get; set; } | Liest und setzt den Typ der Auswahlregel. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetCellAreas](../../aspose.cells.pivot/pivotarea/getcellareas/)() | Liest Zellbereiche dieses PivotArea. |
| [Select](../../aspose.cells.pivot/pivotarea/select/)(PivotFieldType, int, PivotTableSelectionType) | Wählen Sie den Bereich mit Filtern aus. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield)(PivotFieldType, PivotField) | Wählen Sie ein Feld im Bereich als Bereich aus. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield_1)(PivotFieldType, string) | Wählen Sie ein Feld im Bereich als Bereich aus. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaDemo
    {
        public static void PivotAreaExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2021;
            worksheet.Cells[3, 1].Value = 2022;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Fügen Sie der Arbeitsmappe eine PivotTable hinzu
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Erstellen Sie eine PivotArea-Instanz
            PivotArea pivotArea = new PivotArea(pivotTable);

            // Setzen Sie Eigenschaften des PivotArea
            pivotArea.OnlyData = true;
            pivotArea.OnlyLabel = false;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.IsOutline = false;

            // Verwenden Sie die Select-Methode, um einen bestimmten Bereich auszuwählen
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotAreaExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


