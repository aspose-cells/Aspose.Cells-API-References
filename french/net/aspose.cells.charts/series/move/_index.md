---
title: "Series.Move"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Series. Déplace la série vers le haut ou vers le bas"
type: docs
url: /fr/net/aspose.cells.charts/series/move/
---
## Series.Move method

Déplace la série vers le haut ou vers le bas.

```csharp
public void Move(int count)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nombre | Int32 | Le nombre de déplacements vers le haut ou vers le bas. Déplacez la série vers le haut si cette valeur est inférieure à zéro ; déplacez la série vers le bas si elle est supérieure à zéro. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesMethodMoveWithInt32Demo
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
            
            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter des séries au graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Obtenir la première série
            Series series = chart.NSeries[0];
            
            try
            {
                // Appelez la méthode Move avec le paramètre Int32
                series.Move(1);
                
                Console.WriteLine("Series moved successfully by 1 position");
                
                // Montrez l'effet en changeant le nom de la série
                series.Name = "Moved Series";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("SeriesMethodMoveWithInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


