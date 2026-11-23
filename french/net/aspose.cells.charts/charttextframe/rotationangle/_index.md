---
title: "ChartTextFrame.RotationAngle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartTextFrame. Représente l'angle de rotation du texte"
type: docs
url: /fr/net/aspose.cells.charts/charttextframe/rotationangle/
---
## ChartTextFrame.RotationAngle property

Représente l'angle de rotation du texte.

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

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyRotationAngleDemo
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

            // Ajouter un graphique et définir sa plage de données
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir l'angle de rotation du titre de l'axe des valeurs
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.RotationAngle = 45;

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


