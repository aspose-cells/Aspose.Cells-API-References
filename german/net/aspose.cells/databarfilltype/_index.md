---
title: "Enum DataBarFillType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DataBarFillType enum. Gibt an, wie ein Datenbalken mit Farbe gefüllt wird."
type: docs
url: /de/net/aspose.cells/databarfilltype/
---
## DataBarFillType enumeration

Gibt an, wie ein Datenbalken mit Farbe gefüllt wird.

```csharp
public enum DataBarFillType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Solid | `0` | Der Datenbalken ist mit einer Vollfarbe gefüllt. |
| Gradient | `1` | Der Datenbalken ist mit einem Farbverlauf gefüllt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarFillTypeDemo
    {
        public static void DataBarFillTypeExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zum Arbeitsbuch hinzufügen
            Worksheet sheet = workbook.Worksheets[0];

            // Fügt eine leere bedingte Formatierung hinzu
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Setzt den Bereich für die bedingte Formatierung.
            CellArea ca = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Fügt Bedingung hinzu
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Databar abrufen
            DataBar dataBar = cond.DataBar;

            // Databar-Eigenschaften festlegen
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Zellwerte einfügen
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Die Excel-Datei speichern
            workbook.Save("DataBarFillTypeExample.xlsx");
            workbook.Save("DataBarFillTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


