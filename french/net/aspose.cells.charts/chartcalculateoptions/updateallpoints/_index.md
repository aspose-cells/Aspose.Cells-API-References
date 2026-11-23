---
title: "ChartCalculateOptions.UpdateAllPoints"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartCalculateOptions. Indique s’il faut mettre à jour tous les points de données lors du calcul du graphique. Valeur par défaut False. Lorsque vous souhaitez obtenir la valeur de chaque point de données dans le graphique, définissez-la sur true. Si ce paramètre est défini sur True, de nouveaux points de données peuvent être générés lors du calcul du graphique. Cela peut augmenter la taille du fichier Excel."
type: docs
url: /fr/net/aspose.cells.charts/chartcalculateoptions/updateallpoints/
---
## ChartCalculateOptions.UpdateAllPoints property

Indique s'il faut mettre à jour tous les points de données lors du calcul du graphique. Valeur par défaut : False. Lorsque vous souhaitez obtenir la valeur de chaque point de données du graphique spécifiquement, réglez-le sur true. Si ce paramètre est défini sur True, de nouveaux points de données peuvent être générés lors du calcul du graphique. Cela peut augmenter la taille du fichier Excel.

```csharp
public bool UpdateAllPoints { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCalculateOptionsPropertyUpdateAllPointsDemo
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
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(400);
            worksheet.Cells["C3"].PutValue(500);
            worksheet.Cells["C4"].PutValue(600);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Activer les étiquettes de données
            foreach (Aspose.Cells.Charts.Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
            }

            // Calculer le graphique avec l’option UpdateAllPoints
            chart.Calculate(new Aspose.Cells.Charts.ChartCalculateOptions() { UpdateAllPoints = true });

            // Afficher certaines valeurs d’étiquettes de données pour démontrer le résultat
            Console.WriteLine("Series1 Point1 Label: " + chart.NSeries[0].Points[0].DataLabels.Text);
            Console.WriteLine("Series2 Point2 Label: " + chart.NSeries[1].Points[1].DataLabels.Text);
        }
    }
}
```

### Voir aussi

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


