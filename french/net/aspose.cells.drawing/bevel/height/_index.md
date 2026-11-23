---
title: "Bevel.Height"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Bevel propriété. Obtient et définit la hauteur du biseau ou la distance au-dessus de la forme où il est appliqué. En unité de points"
type: docs
url: /fr/net/aspose.cells.drawing/bevel/height/
---
## Bevel.Height property

Obtient et définit la hauteur du biseau, ou la distance au-dessus de la forme où il est appliqué. En unité de points.

```csharp
public double Height { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class BevelPropertyHeightDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(1500);

            // Ajouter un graphique à colonnes 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Accéder au format 3D de la zone de tracé
            Format3D format3D = chart.PlotArea.ShapeProperties.Format3D;

            // Configurer le biseau supérieur avec la propriété Height
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.ArtDeco;
            topBevel.Width = 8;
            topBevel.Height = 4.5; // Demonstrating Height property usage

            // Enregistrez le classeur
            workbook.Save("BevelHeightDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


