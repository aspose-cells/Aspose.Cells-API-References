---
title: "Chart.Move"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Chart method. Déplace le graphique vers un emplacement spécifié"
type: docs
url: /fr/net/aspose.cells.charts/chart/move/
---
## Chart.Move method

Déplace le graphique vers un emplacement spécifié.

```csharp
public void Move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| rightColumn | Int32 | Index de la colonne du coin inférieur droit |
| bottomRow | Int32 | Index de la ligne du coin inférieur droit |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodMoveWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Position originale du graphique
                Console.WriteLine($"Original position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Déplacez le graphique vers une nouvelle position (lignes 10-20, colonnes 2-8)
                chart.Move(10, 2, 20, 8);

                // Afficher la nouvelle position
                Console.WriteLine($"New position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Enregistrez le classeur
                workbook.Save("ChartMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


