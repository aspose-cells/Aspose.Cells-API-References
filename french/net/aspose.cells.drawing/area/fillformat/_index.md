---
title: "Area.FillFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Area. Représente un objet FillFormat qui contient les propriétés de formatage de remplissage pour le graphique ou la forme spécifiés"
type: docs
url: /fr/net/aspose.cells.drawing/area/fillformat/
---
## Area.FillFormat property

Représente un objet `FillFormat` qui contient les propriétés de formatage de remplissage pour le graphique ou la forme spécifiés.

```csharp
public FillFormat FillFormat { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyFillFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenir le troisième point de la première série
            ChartPoint point = chart.NSeries[0].Points[2];
            
            // Définir les propriétés du format de remplissage
            point.Area.FillFormat.Pattern = FillPattern.DashedHorizontal;
            point.Area.FillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.Horizontal, 2);

            // Enregistrez le classeur
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FillFormat](../../fillformat/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


