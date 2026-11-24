---
title: "FillFormat.SetOneColorGradient"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Methode. Setzt die angegebene Füllung auf einen einfarbigen Farbverlauf. Gilt nur für Excel 2007"
type: docs
url: /de/net/aspose.cells.drawing/fillformat/setonecolorgradient/
---
## FillFormat.SetOneColorGradient method

Setzt die angegebene Füllung auf einen einfarbigen Farbverlauf. Gilt nur für Excel 2007.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Farbe | Farbe | Eine Gradientfarbe. |
| Grad | Double | Der Grad des Farbverlaufs. Kann ein Wert von 0.0 (dunkel) bis 1.0 (hell) sein. |
| Stil | GradientStyleType | Gradient-Schattierungsstil. |
| Variante | Int32 | Die Gradientvariante. Kann einen Wert von 1 bis 4 haben, der einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fill Effects entspricht. Wenn style GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Verlauffüllung auf die erste Serie anwenden
            Series series = chart.NSeries[0];
            series.IsColorVaried = false;
            
            // Demonstriere SetOneColorGradient mit spezifischen Parametern
            series.Area.FillFormat.SetOneColorGradient(
                Color.FromArgb(0, 236, 102, 102), // Color
                0.9,                              // Transparency
                Aspose.Cells.Drawing.GradientStyleType.DiagonalDown,    // Gradient style
                2);                                // Variant

            // Speichere die Arbeitsmappe
            workbook.Save("FillFormat_SetOneColorGradient_Output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


