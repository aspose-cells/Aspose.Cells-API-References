---
title: "Chart.GetActualSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode du graphique. Obtient la taille réelle du graphique en pixels."
type: docs
url: /fr/net/aspose.cells.charts/chart/getactualsize/
---
## Chart.GetActualSize method

Obtient la taille réelle du graphique en pixels.

```csharp
public int[] GetActualSize()
```

### Valeur de retour

Taille réelle dans un tableau (largeur et hauteur). [0] correspond à la largeur ; [1] correspond à la hauteur.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodGetActualSizeDemo
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
                // Appelez la méthode GetActualSize.
                int[] actualSize = chart.GetActualSize();
                
                // Afficher le résultat
                Console.WriteLine($"Actual chart size - Width: {actualSize[0]}px, Height: {actualSize[1]}px");
                
                // Montrez l'effet en redimensionnant l'objet graphique.
                chart.ChartObject.Width = actualSize[0];
                chart.ChartObject.Height = actualSize[1];
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetActualSize method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("ChartMethodGetActualSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


