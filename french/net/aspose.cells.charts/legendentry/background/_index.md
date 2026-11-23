---
title: "LegendEntry.Background"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LegendEntry. Obtient et définit le mode d'affichage de l'arrière-plan"
type: docs
url: /fr/net/aspose.cells.charts/legendentry/background/
---
## LegendEntry.Background property

Obtient et définit le mode d'affichage de l'arrière-plan

```csharp
[Obsolete("Use LegendEntry.BackgroundMode property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Remarques

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété LegendEntry.BackgroundMode. Cette propriété sera supprimée 12 mois plus tard depuis JANVIER 2012. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryPropertyBackgroundDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Obtenir la première entrée de légende
                LegendEntry legendEntry = chart.Legend.LegendEntries[0];

                // Afficher la valeur actuelle de la propriété Background
                Console.WriteLine("Current Background value: " + legendEntry.Background);

                // Définir une nouvelle valeur pour Background (puisqu'elle n'est pas en lecture seule)
                legendEntry.Background = BackgroundMode.Opaque;
                Console.WriteLine("Background after setting to Opaque: " + legendEntry.Background);

                // Définir une autre valeur pour Background
                legendEntry.Background = BackgroundMode.Transparent;
                Console.WriteLine("Background after setting to Transparent: " + legendEntry.Background);

                // Enregistrez le classeur
                workbook.Save("LegendEntryBackgroundDemo.xlsx");
                Console.WriteLine("Background property demonstration completed successfully.");
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

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


