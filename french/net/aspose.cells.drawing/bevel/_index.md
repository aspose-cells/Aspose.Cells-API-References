---
title: "Classe Bevel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Bevel. Représente un biseau d'une forme"
type: docs
url: /fr/net/aspose.cells.drawing/bevel/
---
## Bevel class

Représente un biseau d'une forme

```csharp
public class Bevel
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Height](../../aspose.cells.drawing/bevel/height/) { get; set; } | Obtient et définit la hauteur du biseau, ou la distance au-dessus de la forme où il est appliqué. En unité de points. |
| [Type](../../aspose.cells.drawing/bevel/type/) { get; set; } | Obtient et définit le type de biseau prédéfini. |
| [Width](../../aspose.cells.drawing/bevel/width/) { get; set; } | Obtient et définit la largeur du biseau, ou la profondeur dans la forme où il est appliqué. En unité de points. |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class BevelDemo
    {
        public static void RunDemo()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
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

            workbook.CalculateFormula();

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter une série de données au graphique
            chart.NSeries.Add("A1:B4", true);

            // Accéder à la zone de tracé du graphique
            ChartFrame plotArea = chart.PlotArea;

            // Accéder aux propriétés de forme de la zone de tracé
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            // Accéder aux propriétés du format 3D
            Format3D format3D = shapeProperties.Format3D;

            // Accéder aux propriétés du biseau supérieur
            Bevel topBevel = format3D.TopBevel;

            // Définissez la largeur, la hauteur et le type du biseau
            topBevel.Width = 10.0;
            topBevel.Height = 5.0;
            topBevel.Type = BevelPresetType.Circle;

            // Définissez d'autres propriétés de format 3D
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Enregistrez le classeur
            workbook.Save("BevelDemo.xlsx");
            workbook.Save("BevelDemo.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


