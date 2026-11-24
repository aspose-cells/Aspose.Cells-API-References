---
title: "FillFormat.PresetColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Gibt die voreingestellte Farbverlauffarbe für die angegebene Füllung zurück."
type: docs
url: /de/net/aspose.cells.drawing/fillformat/presetcolor/
---
## FillFormat.PresetColor property

Gibt die voreingestellte Farbverlauffarbe für die angegebene Füllung zurück.

```csharp
public GradientPresetType PresetColor { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPresetColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Greifen Sie auf das Füllformat des Diagrammbereichs zu.
            FillFormat fillFormat = chart.ChartArea.Area.FillFormat;

            // Setzen Sie eine voreingestellte Farbverlauffarbe.
            fillFormat.SetPresetColorGradient(GradientPresetType.Ocean, GradientStyleType.DiagonalUp, 2);

            // Zeigen Sie die voreingestellte Farbe an und überprüfen Sie sie.
            Console.WriteLine("Preset Color: " + fillFormat.PresetColor);

            // Speichere die Arbeitsmappe
            workbook.Save("FillFormatPresetColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [GradientPresetType](../../gradientpresettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


