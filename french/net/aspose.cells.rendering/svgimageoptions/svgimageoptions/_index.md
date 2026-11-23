---
title: "SvgImageOptions.SvgImageOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur SvgImageOptions. Ctor"
type: docs
url: /fr/net/aspose.cells.rendering/svgimageoptions/svgimageoptions/
---
## SvgImageOptions constructor

Constructeur.

```csharp
public SvgImageOptions()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Month");
            worksheet.Cells["A2"].PutValue("Jan");
            worksheet.Cells["A3"].PutValue("Feb");
            worksheet.Cells["A4"].PutValue("Mar");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(210);
            worksheet.Cells["B4"].PutValue(150);

            // Créer un graphique linéaire
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Créer SvgImageOptions en utilisant le constructeur
                SvgImageOptions svgOptions = new SvgImageOptions();

                // Configurer les options de rendu SVG
                svgOptions.ImageType = ImageType.Svg; // Explicitly set to SVG
                svgOptions.FitToViewPort = true;
                svgOptions.CssPrefix = "chart-prefix";
                svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

                // Enregistrer le graphique au format SVG avec les options spécifiées
                chart.ToImage("output_chart.svg", svgOptions);

                Console.WriteLine("SVG image saved successfully with specified options.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error generating SVG: {ex.Message}");
            }

            // Enregistrer le classeur pour démontrer les données originales
            workbook.Save("SvgImageOptionsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


