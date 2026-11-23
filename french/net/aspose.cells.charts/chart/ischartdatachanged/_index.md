---
title: "Chart.IsChartDataChanged"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Chart. Détecte si la source de données du graphique a changé"
type: docs
url: /fr/net/aspose.cells.charts/chart/ischartdatachanged/
---
## Chart.IsChartDataChanged method

Détecte si la source de données d'un graphique a changé.

```csharp
public bool IsChartDataChanged()
```

### Valeur de retour

Renvoie true si le graphique a changé, sinon renvoie false

### Remarques

La méthode détecte les changements dans la source de données du graphique avant de rendre le graphique au format image. Lors du premier appel à Chart.toImage, les données sources du graphique (par ex. XValuesParseData, ValuesParseData) seront enregistrées. Avant d'appeler à nouveau la méthode Chart.toImage, appelez la méthode IsChartDataChanged pour vérifier si le graphique doit être re-rendu.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsChartDataChangedDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Vérifier si les données du graphique ont changé (devrait être false initialement)
                bool isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after creation: {isChanged}");

                // Modifier les données du graphique
                worksheet.Cells["B2"].PutValue(15);

                // Vérifier à nouveau si les données du graphique ont changé
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after modification: {isChanged}");

                // Calculer le graphique pour le mettre à jour
                chart.Calculate();

                // Vérifier après le calcul
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after calculation: {isChanged}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsChartDataChanged method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("ChartMethodIsChartDataChangedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


