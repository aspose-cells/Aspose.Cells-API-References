---
title: "SolidFill.Transparency"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SolidFill. Retourne ou définit le degré de transparence de la zone comme une valeur de 0,0 opaque à 1,0 clair"
type: docs
url: /fr/net/aspose.cells.drawing/solidfill/transparency/
---
## SolidFill.Transparency property

Renvoie ou définit le degré de transparence de la zone comme une valeur de 0,0 (opaque) à 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un graphique d'exemple
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // Ajouter une forme pour démontrer la transparence
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating, 
                1000, 1000, 2000, 2000);
            
            // Définissez un remplissage uni avec transparence
            shape.Fill.SolidFill.Color = Color.Blue;
            shape.Fill.SolidFill.Transparency = 0.5; // 50% transparent

            // Ajoutez une autre forme pour comparaison (entièrement opaque)
            Shape shape2 = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating, 
                3000, 1000, 2000, 2000);
            shape2.Fill.SolidFill.Color = Color.Blue;
            shape2.Fill.SolidFill.Transparency = 0; // 0% transparent (fully opaque)

            // Enregistrez le classeur
            workbook.Save("SolidFillTransparencyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


