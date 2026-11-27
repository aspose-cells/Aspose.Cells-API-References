---
title: "FillFormat.SetOneColorGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-metod. Ställer in den angivna fyllningen till en enfärgsgradient. Gäller endast för Excel 2007"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/setonecolorgradient/
---
## FillFormat.SetOneColorGradient method

Ställer in den angivna fyllningen till en enfärgsgradient. Gäller endast för Excel 2007.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| färg | Färg | En gradientfärg. |
| grad | Double | Gradientens grad. Kan vara ett värde från 0,0 (mörk) till 1,0 (ljus). |
| style | GradientStyleType | Gradientskuggningsstil. |
| variant | Int32 | Gradientvarianten. Kan vara ett värde från 1 till 4, motsvarande en av de fyra varianterna på fliken Gradient i dialogrutan Fylleffekter. Om stil är GradientStyle.FromCenter, kan Variant‑argumentet endast vara 1 eller 2. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Tillämpa gradientfyllning på den första serien
            Series series = chart.NSeries[0];
            series.IsColorVaried = false;
            
            // Visa SetOneColorGradient med specifika parametrar
            series.Area.FillFormat.SetOneColorGradient(
                Color.FromArgb(0, 236, 102, 102), // Color
                0.9,                              // Transparency
                Aspose.Cells.Drawing.GradientStyleType.DiagonalDown,    // Gradient style
                2);                                // Variant

            // Spara arbetsboken
            workbook.Save("FillFormat_SetOneColorGradient_Output.xlsx");
        }
    }
}
```

### Se även

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


