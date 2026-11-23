---
title: "Axis.TickLabels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Retourne un objet TickLabels qui représente les libellés des marques de graduation pour l'axe spécifié"
type: docs
url: /fr/net/aspose.cells.charts/axis/ticklabels/
---
## Axis.TickLabels property

Retourne un objet `TickLabels` qui représente les libellés des marques de graduation pour l'axe spécifié.

```csharp
public TickLabels TickLabels { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickLabelsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Accéder aux étiquettes de repère de l'axe des catégories
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            axis.TickLabels.Font.IsBold = true;
            axis.TickLabels.Font.Color = System.Drawing.Color.Red;
            axis.TickLabels.RotationAngle = 45;
            
            // Enregistrez le classeur
            workbook.Save("AxisPropertyTickLabelsDemo_out.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [TickLabels](../../ticklabels/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


