---
title: "SvgImageOptions.FitToViewPort"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SvgImageOptions-egenskap. Om denna egenskap är sann kommer den genererade SVG:n att anpassas till visningsporten"
type: docs
url: /sv/net/aspose.cells.rendering/svgimageoptions/fittoviewport/
---
## SvgImageOptions.FitToViewPort property

Om denna egenskap är sann, kommer den genererade svg att anpassas till visningsporten.

```csharp
public bool FitToViewPort { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsPropertyFitToViewPortDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll celler med exempeldata
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 250;

            // Skapa ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 18, 6);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            chart.Title.Text = "Sales Report";

            // Skapa SVG-renderingsalternativ
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Visa initialt FitToViewPort-värde
            Console.WriteLine($"Initial FitToViewPort: {svgOptions.FitToViewPort}");

            // Modifiera egenskapen och demonstrera effekten
            svgOptions.FitToViewPort = true;
            Console.WriteLine($"Modified FitToViewPort: {svgOptions.FitToViewPort}");

            // Rendera kalkylblad till SVG med olika inställningar
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortEnabled.svg");

            // Valfritt: Skapa jämförelse med inaktiverad FitToViewPort
            svgOptions.FitToViewPort = false;
            renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortDisabled.svg");

            Console.WriteLine("Generated SVG files demonstrate FitToViewPort effect.");
        }
    }
}
```

### Se även

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


