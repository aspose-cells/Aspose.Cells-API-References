---
title: "TickLabels.RotationAngle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TickLabels. Représente l'angle de rotation du texte dans le sens des aiguilles d'une montre"
type: docs
url: /fr/net/aspose.cells.charts/ticklabels/rotationangle/
---
## TickLabels.RotationAngle property

Représente l'angle de rotation du texte dans le sens des aiguilles d'une montre.

```csharp
public int RotationAngle { get; set; }
```

### Remarques

0 : Non pivoté.255 : De haut en bas.-90 : Vers le bas.90 : Vers le haut.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["A3"].PutValue("Category 3");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(200);
            sheet.Cells["B3"].PutValue(300);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Faire pivoter les étiquettes de graduation de l'axe des catégories de 45 degrés
            chart.CategoryAxis.TickLabels.RotationAngle = 45;

            // Enregistrez le classeur
            workbook.Save("TickLabelsRotationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


