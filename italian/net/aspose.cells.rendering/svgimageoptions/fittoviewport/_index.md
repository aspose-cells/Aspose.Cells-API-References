---
title: "SvgImageOptions.FitToViewPort"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SvgImageOptions. se questa proprietà è true il SVG generato si adatterà alla viewport"
type: docs
url: /it/net/aspose.cells.rendering/svgimageoptions/fittoviewport/
---
## SvgImageOptions.FitToViewPort property

Se questa proprietà è true, l'SVG generato si adatterà alla viewport.

```csharp
public bool FitToViewPort { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola le celle con dati di esempio
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 250;

            // Crea un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 18, 6);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            chart.Title.Text = "Sales Report";

            // Crea opzioni di rendering SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Visualizza il valore iniziale di FitToViewPort
            Console.WriteLine($"Initial FitToViewPort: {svgOptions.FitToViewPort}");

            // Modifica la proprietà e dimostra l'effetto
            svgOptions.FitToViewPort = true;
            Console.WriteLine($"Modified FitToViewPort: {svgOptions.FitToViewPort}");

            // Esegui il rendering del foglio di lavoro in SVG con impostazioni diverse
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortEnabled.svg");

            // Opzionale: crea un confronto con FitToViewPort disabilitato
            svgOptions.FitToViewPort = false;
            renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortDisabled.svg");

            Console.WriteLine("Generated SVG files demonstrate FitToViewPort effect.");
        }
    }
}
```

### Vedi anche

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


