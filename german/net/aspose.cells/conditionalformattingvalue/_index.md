---
title: "Klasse ConditionalFormattingValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ConditionalFormattingValue Klasse. Beschreibt die Werte der Interpolationspunkte in einer Farbskala dataBar oder iconSet"
type: docs
url: /de/net/aspose.cells/conditionalformattingvalue/
---
## ConditionalFormattingValue class

Beschreibt die Werte der Interpolationspunkte in einer Gradienten‑Skala, einem DataBar oder einem IconSet.

```csharp
public class ConditionalFormattingValue
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsGTE](../../aspose.cells/conditionalformattingvalue/isgte/) { get; set; } | Abrufen oder Festlegen des Greater Than Or Equal‑Flags. Nur für Icon‑Sets verwenden, bestimmt, ob dieser Schwellenwert den Operator größer‑gleich verwendet. 'false' bedeutet, dass 'größer als' anstelle von 'größer‑gleich' verwendet wird. Der Standardwert ist true. |
| [Type](../../aspose.cells/conditionalformattingvalue/type/) { get; set; } | Abrufen oder Festlegen des Typs dieses bedingten Formatierungswertobjekts. Das Setzen des Typs auf FormatConditionValueType.Min oder FormatConditionValueType.Max setzt "Value" automatisch auf null. |
| [Value](../../aspose.cells/conditionalformattingvalue/value/) { get; set; } | Abrufen oder Festlegen des Werts dieses bedingten Formatierungswertobjekts. Es sollte zusammen mit Type verwendet werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingValueDemo
    {
        public static void ConditionalFormattingValueExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügt eine leere bedingte Formatierung hinzu
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Setzt den Bereich der bedingten Formatierung
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Fügt Bedingung hinzu
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Festlegen von Eigenschaften für ColorScale
            fc.ColorScale.Is3ColorScale = true;

            // Festlegen des Minimalwerts
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinCfvo.Value = null;
            fc.ColorScale.MinColor = Color.Blue;

            // Festlegen des Mittelwerts
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;

            // Festlegen des Maximalwerts
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxCfvo.Value = null;
            fc.ColorScale.MaxColor = Color.Red;

            // Speichere die Arbeitsmappe
            workbook.Save("ConditionalFormattingValueExample.xlsx");
            workbook.Save("ConditionalFormattingValueExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


