---
title: "Trendline.IsNameAuto"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Trendline. Retourne si Microsoft Excel détermine automatiquement le nom de la courbe de tendance"
type: docs
url: /fr/net/aspose.cells.charts/trendline/isnameauto/
---
## Trendline.IsNameAuto property

Renvoie si Microsoft Excel détermine automatiquement le nom de la courbe de tendance.

```csharp
public bool IsNameAuto { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyIsNameAutoDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter une série au graphique
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Ajouter une courbe de tendance - modifié pour garantir la création correcte de l'objet Trendline
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Démontrer la propriété IsNameAuto
            Console.WriteLine("Initial IsNameAuto value: " + trendline.IsNameAuto);
            
            // Définir un nom personnalisé (désactive le nommage automatique)
            trendline.Name = "Custom Trendline Name";
            Console.WriteLine("After setting custom name, IsNameAuto: " + trendline.IsNameAuto);
            
            // Réinitialiser au nom automatique
            trendline.IsNameAuto = true;
            Console.WriteLine("After setting IsNameAuto=true, Name: " + trendline.Name);
        }
    }
}
```

### Voir aussi

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


