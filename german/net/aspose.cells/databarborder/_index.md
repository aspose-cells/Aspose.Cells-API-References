---
title: "Klasse DataBarBorder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DataBarBorder Klasse. Stellt die Grenze der Datenbalken dar, die durch eine bedingte Formatierungsregel festgelegt werden."
type: docs
url: /de/net/aspose.cells/databarborder/
---
## DataBarBorder class

Stellt den Rand der Datenbalken dar, die durch eine bedingte Formatierungsregel festgelegt sind.

```csharp
public class DataBarBorder
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Color](../../aspose.cells/databarborder/color/) { get; set; } | Liest oder setzt die Farbe der Grenze der Datenbalken, die durch eine bedingte Formatierungsregel festgelegt sind. |
| [Type](../../aspose.cells/databarborder/type/) { get; set; } | Liest oder setzt den Typ der Grenze der Datenbalken, die durch eine bedingte Formatierungsregel festgelegt sind. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarBorderDemo
    {
        public static void DataBarBorderExample()
        {
            // Erstellen einer neuen Arbeitsmappe
            Workbook workbook = new Workbook();
            // Zugriff auf das erste Arbeitsblatt in der Arbeitsmappe
            Worksheet worksheet = workbook.Worksheets[0];

            // Hinzufügen einiger Beispieldaten zum Arbeitsblatt
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(80);
            worksheet.Cells["A4"].PutValue(60);
            worksheet.Cells["A5"].PutValue(30);

            // Hinzufügen einer leeren bedingten Formatierung
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Definieren eines Zellbereichs für bedingte Formatierung
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Hinzufügen einer Bedingung vom Typ DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition formatCondition = fcs[conditionIndex];

            // Zugriff auf die DataBar
            DataBar dataBar = formatCondition.DataBar;

            // Festlegen der DataBar-Eigenschaften
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 0;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MaxCfvo.Value = 100;
            dataBar.ShowValue = true;

            // Zugriff auf und Festlegen der DataBarBorder-Eigenschaften
            DataBarBorder dataBarBorder = dataBar.BarBorder;
            dataBarBorder.Type = DataBarBorderType.Solid;
            dataBarBorder.Color = Color.Black;

            // Die Excel-Datei speichern
            workbook.Save("DataBarBorderExample.xlsx");
            workbook.Save("DataBarBorderExample.pdf");

            Console.WriteLine("DataBar border example created successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


