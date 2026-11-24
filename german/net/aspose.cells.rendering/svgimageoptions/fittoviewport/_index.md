---
title: "SvgImageOptions.FitToViewPort"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SvgImageOptions Eigenschaft. Wenn diese Eigenschaft true ist, passt das erzeugte SVG an den Viewport"
type: docs
url: /de/net/aspose.cells.rendering/svgimageoptions/fittoviewport/
---
## SvgImageOptions.FitToViewPort property

Wenn diese Eigenschaft wahr ist, passt das erzeugte SVG an den Viewport an.

```csharp
public bool FitToViewPort { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zellen mit Beispieldaten füllen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 250;

            // Erstelle ein Säulendiagramm
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 18, 6);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            chart.Title.Text = "Sales Report";

            // Erstelle SVG-Renderoptionen
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Zeige den anfänglichen FitToViewPort-Wert an
            Console.WriteLine($"Initial FitToViewPort: {svgOptions.FitToViewPort}");

            // Modifiziere die Eigenschaft und demonstriere die Wirkung
            svgOptions.FitToViewPort = true;
            Console.WriteLine($"Modified FitToViewPort: {svgOptions.FitToViewPort}");

            // Render das Arbeitsblatt zu SVG mit unterschiedlichen Einstellungen
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortEnabled.svg");

            // Optional: Erstelle einen Vergleich mit deaktiviertem FitToViewPort
            svgOptions.FitToViewPort = false;
            renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortDisabled.svg");

            Console.WriteLine("Generated SVG files demonstrate FitToViewPort effect.");
        }
    }
}
```

### Siehe auch

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


