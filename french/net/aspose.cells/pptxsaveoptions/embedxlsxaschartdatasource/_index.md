---
title: "PptxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PptxSaveOptions. Indique si un fichier xlsx doit être intégré comme source de données du graphique"
type: docs
url: /fr/net/aspose.cells/pptxsaveoptions/embedxlsxaschartdatasource/
---
## PptxSaveOptions.EmbedXlsxAsChartDataSource property

Indique s'il faut intégrer un fichier xlsx comme source de données du graphique.

```csharp
public bool EmbedXlsxAsChartDataSource { get; set; }
```

### Remarques

La valeur par défaut est true.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PptxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d'exemple avec des données de graphique
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Ajouter un graphique pour démontrer l'effet de la propriété
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Créer une instance de PptxSaveOptions
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // Afficher la valeur par défaut de EmbedXlsxAsChartDataSource
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Définir la propriété sur true pour démontrer son utilisation
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Enregistrer le classeur au format PPTX avec l'option activée
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with EmbedXlsxAsChartDataSource enabled");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


