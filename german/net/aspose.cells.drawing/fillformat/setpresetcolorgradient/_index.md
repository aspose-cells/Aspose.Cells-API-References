---
title: "FillFormat.SetPresetColorGradient"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Methode. Setzt die angegebene Füllung auf einen voreingestellten Farbverlauf. Gilt nur für Excel 2007."
type: docs
url: /de/net/aspose.cells.drawing/fillformat/setpresetcolorgradient/
---
## FillFormat.SetPresetColorGradient method

Setzt die angegebene Füllung auf einen voreingestellten Farbverlauf. Gilt nur für Excel 2007.

```csharp
public void SetPresetColorGradient(GradientPresetType presetColor, GradientStyleType style, 
    int variant)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| presetColor | GradientPresetType | Voreingestellter Farbtyp |
| Stil | GradientStyleType | Gradient-Schattierungsstil. |
| Variante | Int32 | Die Gradientvariante. Kann einen Wert von 1 bis 4 haben, der einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fill Effects entspricht. Wenn style GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetPresetColorGradientWithGradientPresetTypeGradientStylDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Item {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 10);
            }

            // Diagramm erstellen
            int chartIndex = sheet.Charts.Add(ChartType.Column, 8, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Farbverlauffüllung anwenden.
            FillFormat fillFormat = chart.PlotArea.Area.FillFormat;
            fillFormat.SetPresetColorGradient(GradientPresetType.Daybreak, GradientStyleType.Vertical, 1);

            // Speichere die Arbeitsmappe
            workbook.Save("SetPresetColorGradientDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [GradientPresetType](../../gradientpresettype/)
* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


