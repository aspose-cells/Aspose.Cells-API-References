---
title: "Klasse ColorScale"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ColorScale Klasse. Beschreibe die ColorScale‑Bedingte‑Formatierungs‑Regel. Diese bedingte Formatierungsregel erstellt eine abgestufte Farbskala in den Zellen"
type: docs
url: /de/net/aspose.cells/colorscale/
---
## ColorScale class

Beschreibt die ColorScale-Bedingte-Formatierungsregel. Diese bedingte Formatierungsregel erstellt eine abgestufte Farbskala in den Zellen.

```csharp
public class ColorScale
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Is3ColorScale](../../aspose.cells/colorscale/is3colorscale/) { get; set; } | Gibt an, ob die bedingte Formatierung eine 3‑Farbskala ist. |
| [MaxCfvo](../../aspose.cells/colorscale/maxcfvo/) { get; } | Lese oder setze das Maximalwert‑Objekt dieser ColorScale. Es kann nicht null oder ein CFValueObject mit dem Typ FormatConditionValueType.Min zugewiesen werden. |
| [MaxColor](../../aspose.cells/colorscale/maxcolor/) { get; set; } | Lese oder setze die Verlaufsfarbe für den Maximalwert im Bereich. |
| [MidCfvo](../../aspose.cells/colorscale/midcfvo/) { get; } | Abrufen oder Festlegen des Midwertobjekts dieses ColorScale. CFValueObject mit dem Typ FormatConditionValueType.Max oder FormatConditionValueType.Min kann nicht dafür festgelegt werden. |
| [MidColor](../../aspose.cells/colorscale/midcolor/) { get; set; } | Abrufen oder Festlegen der Verlaufsfarbe für den mittleren Wert im Bereich. |
| [MinCfvo](../../aspose.cells/colorscale/mincfvo/) { get; } | Abrufen oder Festlegen des Minimalwertobjekts dieses ColorScale. Null oder CFValueObject mit dem Typ FormatConditionValueType.Max kann nicht dafür festgelegt werden. |
| [MinColor](../../aspose.cells/colorscale/mincolor/) { get; set; } | Abrufen oder Festlegen der Verlaufsfarbe für den Minimalwert im Bereich. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColorScaleDemo
    {
        public static void ColorScaleExample()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // Eine bedingte Formatierungsregel hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 9 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Zugriff auf das ColorScale-Objekt
            ColorScale colorScale = fc.ColorScale;

            // Eigenschaften für das ColorScale festlegen
            colorScale.Is3ColorScale = true;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // Festlegen der Minimal-, Mittel- und Maximalwertobjekte
            ConditionalFormattingValue minCfvo = colorScale.MinCfvo;
            minCfvo.Type = FormatConditionValueType.Min;
            minCfvo.Value = null;

            ConditionalFormattingValue midCfvo = colorScale.MidCfvo;
            midCfvo.Type = FormatConditionValueType.Percentile;
            midCfvo.Value = 50;

            ConditionalFormattingValue maxCfvo = colorScale.MaxCfvo;
            maxCfvo.Type = FormatConditionValueType.Max;
            maxCfvo.Value = null;

            // Speichere die Arbeitsmappe
            workbook.Save("ColorScaleExample.xlsx");
            workbook.Save("ColorScaleExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


