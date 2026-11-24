---
title: "Enum PivotFieldDataDisplayFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotFieldDataDisplayFormat enum. Stellt das Datenanzeigeformat im Datenfeld der PivotTable dar"
type: docs
url: /de/net/aspose.cells.pivot/pivotfielddatadisplayformat/
---
## PivotFieldDataDisplayFormat enumeration

Stellt das Anzeigeformat der Daten im Datenfeld einer PivotTable dar.

```csharp
public enum PivotFieldDataDisplayFormat
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Normal | `0` | Stellt das normale Anzeigeformat dar. |
| DifferenceFrom | `1` | Stellt das Anzeigeformat für Unterschiede dar. |
| PercentageOf | `2` | Stellt den Prozentsatz des Anzeigeformats dar. |
| PercentageDifferenceFrom | `3` | Stellt die prozentuale Differenz zum Anzeigeformat dar. |
| RunningTotalIn | `4` | Stellt den laufenden Gesamtwert im Anzeigeformat dar. |
| PercentageOfRow | `5` | Stellt den Prozentsatz des Zeilenanzeigeformats dar. |
| PercentageOfColumn | `6` | Stellt den Prozentsatz des Spaltenanzeigeformats dar. |
| PercentageOfTotal | `7` | Stellt den Prozentsatz des Gesamtanzeigeformats dar. |
| Index | `8` | Stellt das Indexanzeigeformat dar. |
| PercentageOfParentRowTotal | `9` | Stellt den Prozentsatz des übergeordneten Zeilengesamtanzeigeformats dar. |
| PercentageOfParentColumnTotal | `10` | Stellt den Prozentsatz des übergeordneten Spaltengesamtanzeigeformats dar. |
| PercentageOfParentTotal | `11` | Stellt den Prozentsatz des übergeordneten Gesamteanzeigeformats dar. |
| PercentageOfRunningTotalIn | `12` | Stellt den Prozentsatz des laufenden Gesamtwerts im Anzeigeformat dar. |
| RankSmallestToLargest | `13` | Stellt das Anzeigeformat von klein nach groß dar. |
| RankLargestToSmallest | `14` | Stellt das Anzeigeformat von groß nach klein dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDataDisplayFormatDemo
    {
        public static void PivotFieldDataDisplayFormatExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

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
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Setzt den Pivot-Tabellenstil
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Attribute des PivotField ändern
            PivotField dataField = pivot.DataFields[0];
            dataField.DisplayName = "custom display name";

            // Setzt DataDisplayFormat
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;

            // Aktualisieren und Daten berechnen
            pivot.RefreshData();
            pivot.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldDataDisplayFormatExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


