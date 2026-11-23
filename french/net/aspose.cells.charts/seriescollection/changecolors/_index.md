---
title: "SeriesCollection.ChangeColors"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SeriesCollection. Définit une palette monochrome pour les séries du graphique"
type: docs
url: /fr/net/aspose.cells.charts/seriescollection/changecolors/
---
## SeriesCollection.ChangeColors method

Définit la palette monochrome pour les séries du graphique.

```csharp
public void ChangeColors(ChartColorPaletteType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ChartColorPaletteType | Le type monochrome. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodChangeColorsWithChartColorPaletDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Remplir certaines données pour le graphique
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["A2"].PutValue("Jan");
            ws.Cells["A3"].PutValue("Feb");
            ws.Cells["A4"].PutValue("Mar");

            ws.Cells["B1"].PutValue("Series1");
            ws.Cells["B2"].PutValue(10);
            ws.Cells["B3"].PutValue(20);
            ws.Cells["B4"].PutValue(30);

            ws.Cells["C1"].PutValue("Series2");
            ws.Cells["C2"].PutValue(15);
            ws.Cells["C3"].PutValue(25);
            ws.Cells["C4"].PutValue(35);

            // Ajouter un graphique en colonnes
            int chartIdx = ws.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = ws.Charts[chartIdx];

            // Définir la plage de données pour la série
            chart.NSeries.Add("B1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenir la collection de séries
            SeriesCollection seriesColl = chart.NSeries;

            try
            {
                // Modifier la palette de couleurs de toutes les séries dans la collection.
                // Utilisez un cast numérique vers une valeur d'énumération valide (p. ex., 0) pour éviter les noms de membres d'énumération dépendants.
                seriesColl.ChangeColors((ChartColorPaletteType)0);

                Console.WriteLine("ChangeColors method invoked successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error invoking ChangeColors: {ex.Message}");
            }

            // Enregistrez le classeur pour vérifier le résultat
            workbook.Save("SeriesCollection_ChangeColors_Demo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ChartColorPaletteType](../../chartcolorpalettetype/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


