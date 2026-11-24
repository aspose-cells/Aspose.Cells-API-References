---
title: "Klasse ConditionalFormattingResult"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ConditionalFormattingResult Klasse. Stellt das Ergebnis der bedingten Formatierung dar, die auf eine Zelle angewendet wird"
type: docs
url: /de/net/aspose.cells/conditionalformattingresult/
---
## ConditionalFormattingResult class

Stellt das Ergebnis der bedingten Formatierung dar, die auf eine Zelle angewendet wird.

```csharp
public class ConditionalFormattingResult
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ColorScaleResult](../../aspose.cells/conditionalformattingresult/colorscaleresult/) { get; } | Liefert die Anzeigefarbe der Farbskala. |
| [ConditionalFormattingColorScale](../../aspose.cells/conditionalformattingresult/conditionalformattingcolorscale/) { get; } | Liefert das ColorScale-Objekt. |
| [ConditionalFormattingDataBar](../../aspose.cells/conditionalformattingresult/conditionalformattingdatabar/) { get; } | Liefert das DataBar-Objekt. |
| [ConditionalFormattingIcon](../../aspose.cells/conditionalformattingresult/conditionalformattingicon/) { get; } | Liefert das Bild des Symbolsatzes. |
| [ConditionalStyle](../../aspose.cells/conditionalformattingresult/conditionalstyle/) { get; } | Liefert den Stil des bedingten Ergebnisses. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingResultDemo
    {
        public static void ConditionalFormattingResultExample()
        {
            // Instanziieren Sie ein Arbeitsmappen-Objekt
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

            // Setzen Sie ColorScale-Eigenschaften
            fc.ColorScale.Is3ColorScale = true;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxColor = Color.Green;

            // Wenden Sie einige Werte auf die Zellen an
            for (int i = 0; i <= 10; i++)
            {
                for (int j = 0; j <= 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // Holen Sie das Ergebnis der bedingten Formatierung für eine bestimmte Zelle
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult cfr = cell.GetConditionalFormattingResult();

            // Greifen Sie auf die Eigenschaften von ConditionalFormattingResult zu
            Style conditionalStyle = cfr.ConditionalStyle;
            ConditionalFormattingIcon icon = cfr.ConditionalFormattingIcon;
            DataBar dataBar = cfr.ConditionalFormattingDataBar;
            ColorScale colorScale = cfr.ConditionalFormattingColorScale;
            Color colorScaleResult = cfr.ColorScaleResult;

            // Zeigen Sie einige der Eigenschaften an
            Console.WriteLine("Conditional Style Background Color: " + (conditionalStyle != null ? conditionalStyle.BackgroundColor : Color.Empty));
            Console.WriteLine("Conditional Formatting Icon Type: " + (icon != null ? icon.Type.ToString() : "No Icon"));
            Console.WriteLine("Conditional Formatting DataBar Color: " + (dataBar != null ? dataBar.Color.ToString() : "No DataBar"));
            Console.WriteLine("Conditional Formatting ColorScale Min Color: " + (colorScale != null ? colorScale.MinColor.ToString() : "No ColorScale"));
            Console.WriteLine("Color Scale Result: " + colorScaleResult);

            // Speichere die Arbeitsmappe
            workbook.Save("ConditionalFormattingResultExample.xlsx");
            workbook.Save("ConditionalFormattingResultExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


