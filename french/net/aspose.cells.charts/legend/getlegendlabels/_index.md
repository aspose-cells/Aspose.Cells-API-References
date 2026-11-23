---
title: "Legend.GetLegendLabels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Legend. Obtient les libellés des entrées de légende après l'appel de la méthode Chart.Calculate"
type: docs
url: /fr/net/aspose.cells.charts/legend/getlegendlabels/
---
## Legend.GetLegendLabels method

Obtient les étiquettes des entrées de légende après l'appel de la méthode Chart.Calculate().

```csharp
public string[] GetLegendLabels()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendMethodGetLegendLabelsDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Calculer le graphique
            chart.Calculate();
            
            // Obtenir les libellés de la légende
            string[] legendLabels = chart.Legend.GetLegendLabels();
            
            // Afficher les libellés de la légende
            Console.WriteLine("Legend Labels:");
            foreach (string label in legendLabels)
            {
                Console.WriteLine(label);
            }
        }
    }
}
```

### Voir aussi

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


