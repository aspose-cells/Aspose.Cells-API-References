---
title: "Area.ForegroundColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Area. Obtient ou définit la couleur de premier plan"
type: docs
url: /fr/net/aspose.cells.drawing/area/foregroundcolor/
---
## Area.ForegroundColor property

Obtient ou définit la couleur de premier plan.

```csharp
public Color ForegroundColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyForegroundColorDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définissez des couleurs de premier plan différentes pour chaque zone de série
            chart.NSeries[0].Area.ForegroundColor = Color.FromArgb(79, 129, 189);
            chart.NSeries[1].Area.ForegroundColor = Color.FromArgb(192, 80, 77);

            // Enregistrez le classeur
            workbook.Save("AreaForegroundColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


