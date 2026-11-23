---
title: "SvgImageOptions.CssPrefix"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SvgImageOptions. Obtient et définit le préfixe du nom CSS dans le SVG ; la valeur par défaut est une chaîne vide"
type: docs
url: /fr/net/aspose.cells.rendering/svgimageoptions/cssprefix/
---
## SvgImageOptions.CssPrefix property

Obtient et définit le préfixe du nom CSS dans le SVG, la valeur par défaut est une chaîne vide.

```csharp
public string CssPrefix { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SvgImageOptionsPropertyCssPrefixDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue(2019);
            worksheet.Cells["A3"].PutValue(2020);
            worksheet.Cells["A4"].PutValue(2021);
            worksheet.Cells["A5"].PutValue(2022);

            worksheet.Cells["B2"].PutValue(4500);
            worksheet.Cells["B3"].PutValue(4900);
            worksheet.Cells["B4"].PutValue(5200);
            worksheet.Cells["B5"].PutValue(6100);

            // Créer un graphique linéaire
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B5", true);

            // Créer des options d'image SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Afficher le préfixe CSS actuel
            Console.WriteLine("Current CssPrefix value: " + svgOptions.CssPrefix);

            // Définir un nouveau préfixe CSS
            svgOptions.CssPrefix = "chart-prefix-";

            // Démontrer la génération SVG avec un préfixe CSS personnalisé
            string outputPath = "output_chart.svg";
            chart.ToImage(outputPath, svgOptions);

            Console.WriteLine("Chart saved as SVG with custom CSS prefix.");
        }
    }
}
```

### Voir aussi

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


