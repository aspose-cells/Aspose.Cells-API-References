---
title: "Chart.IsCellReferedByChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Chart. Retourne si la cellule est référencée par le graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/iscellreferedbychart/
---
## Chart.IsCellReferedByChart method

Renvoie si la cellule est référencée par le graphique.

```csharp
public bool IsCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | L'index de la feuille. -1 signifie la feuille de calcul qui contient le graphique actuel. |
| rowIndex | Int32 | L'index de la ligne |
| columnIndex | Int32 | L'index de colonne |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodIsCellReferedByChartWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
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
            
            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Vérifier si la cellule est référencée par le graphique
            bool isReferred = chart.IsCellReferedByChart(0, 1, 0); // Check if B2 is referred
            Console.WriteLine("Is cell B2 referred by chart: " + isReferred);
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


