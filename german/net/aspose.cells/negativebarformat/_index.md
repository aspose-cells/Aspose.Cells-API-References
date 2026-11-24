---
title: "Klasse NegativeBarFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.NegativeBarFormat Klasse. Stellt die Farbeinstellungen der Datenbalken für negative Werte dar, die durch eine Datenbalken-Bedingte-Formatierungsregel definiert sind."
type: docs
url: /de/net/aspose.cells/negativebarformat/
---
## NegativeBarFormat class

Stellt die Farbeinstellungen der Datenbalken für negative Werte dar, die durch eine Datenbalken‑Bedingte‑Formatierungsregel definiert sind.

```csharp
public class NegativeBarFormat
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BorderColor](../../aspose.cells/negativebarformat/bordercolor/) { get; set; } | Liest oder setzt ein FormatColor-Objekt, das Sie verwenden können, um die Rahmenfarbe für negative Datenbalken festzulegen. |
| [BorderColorType](../../aspose.cells/negativebarformat/bordercolortype/) { get; set; } | Gibt an, ob die gleiche Rahmenfarbe wie bei positiven Datenbalken verwendet werden soll. |
| [Color](../../aspose.cells/negativebarformat/color/) { get; set; } | Liest oder setzt ein FormatColor-Objekt, das Sie verwenden können, um die Füllfarbe für negative Datenbalken festzulegen. |
| [ColorType](../../aspose.cells/negativebarformat/colortype/) { get; set; } | Liest oder setzt, ob die gleiche Füllfarbe wie bei positiven Datenbalken verwendet werden soll. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class NegativeBarFormatDemo
    {
        public static void NegativeBarFormatExample()
        {
            // Instanziiere ein Workbook-Objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügt eine leere bedingte Formatierung hinzu
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Setzt den Bereich der bedingten Formatierung
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Fügt eine Bedingung für DataBar hinzu
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Erhalte DataBar und setze seine Eigenschaften
            DataBar dataBar = fc.DataBar;
            dataBar.Color = Color.Orange;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            // Konfiguriere die Eigenschaften von NegativeBarFormat
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = Color.White;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = Color.Yellow;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;

            // Setze einige Werte in die Zellen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);

            // Speichere die Arbeitsmappe
            workbook.Save("NegativeBarFormatExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


