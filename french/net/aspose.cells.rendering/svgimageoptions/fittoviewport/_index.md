---
title: "SvgImageOptions.FitToViewPort"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SvgImageOptions. si cette propriété est vraie, le svg généré s'adaptera à la fenêtre d'affichage"
type: docs
url: /fr/net/aspose.cells.rendering/svgimageoptions/fittoviewport/
---
## SvgImageOptions.FitToViewPort property

Si cette propriété est vraie, le SVG généré s’ajustera à la zone d’affichage.

```csharp
public bool FitToViewPort { get; set; }
```

### Exemples

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
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir les cellules avec des données d'exemple
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 250;

            // Créer un graphique à colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 18, 6);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            chart.Title.Text = "Sales Report";

            // Créer des options de rendu SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Afficher la valeur initiale de FitToViewPort
            Console.WriteLine($"Initial FitToViewPort: {svgOptions.FitToViewPort}");

            // Modifier la propriété et démontrer l'effet
            svgOptions.FitToViewPort = true;
            Console.WriteLine($"Modified FitToViewPort: {svgOptions.FitToViewPort}");

            // Rendre la feuille de calcul en SVG avec différents paramètres
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortEnabled.svg");

            // Optionnel : créer une comparaison avec FitToViewPort désactivé
            svgOptions.FitToViewPort = false;
            renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortDisabled.svg");

            Console.WriteLine("Generated SVG files demonstrate FitToViewPort effect.");
        }
    }
}
```

### Voir aussi

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


