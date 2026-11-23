---
title: "DataLabels.ApplyFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DataLabels. Appliquer la police des étiquettes de données à tous les nœuds enfants"
type: docs
url: /fr/net/aspose.cells.charts/datalabels/applyfont/
---
## DataLabels.ApplyFont method

Applique la police des étiquettes de données à tous les nœuds enfants.

```csharp
public void ApplyFont()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsMethodApplyFontDemo
    {
        public static void Run()
        {
            // Créer un classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Afficher les étiquettes de données
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Définir une nouvelle couleur de police pour les étiquettes de données
            Color newColor = Color.Green;
            series.DataLabels.Font.Color = newColor;
            
            // Appliquer les paramètres de police à toutes les étiquettes de données
            series.DataLabels.ApplyFont();
            
            // Enregistrez le classeur
            workbook.Save("DataLabelsApplyFontDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


