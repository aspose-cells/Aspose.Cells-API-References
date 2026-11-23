---
title: "Axis.CustomUnit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Spécifie une valeur personnalisée pour l'unité d'affichage"
type: docs
url: /fr/net/aspose.cells.charts/axis/customunit/
---
## Axis.CustomUnit property

Spécifie une valeur personnalisée pour l'unité d'affichage.

```csharp
[Obsolete("Use Axis.CustomDisplayUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustomUnit { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété Axis.CustomDisplayUnit. Cette propriété sera supprimée 12 mois plus tard, à compter de février 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustomUnitDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Accéder à l'axe des valeurs
                Axis valueAxis = chart.ValueAxis;

                // Définir l'unité d'affichage sur personnalisé
                valueAxis.DisplayUnit = DisplayUnitType.Custom;

                // Définir la valeur de l'unité d'affichage personnalisée
                valueAxis.CustomDisplayUnit = 1000000;

                // Afficher la valeur de la propriété CustomUnit (propriété obsolète)
                Console.WriteLine("CustomUnit value: " + valueAxis.CustomUnit);

                // Enregistrez le classeur
                workbook.Save("AxisPropertyCustomUnitDemo.xlsx");
                Console.WriteLine("CustomUnit has been demonstrated");
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

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


