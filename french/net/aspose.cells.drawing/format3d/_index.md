---
title: "Classe Format3D"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Format3D. Cette classe spécifie les propriétés de forme 3D pour un élément de graphique ou une forme"
type: docs
url: /fr/net/aspose.cells.drawing/format3d/
---
## Format3D class

Cette classe spécifie les propriétés de forme 3D pour un élément de graphique ou une forme.

```csharp
public class Format3D
```

## Propriétés

| Nom | Description |
| --- | --- |
| [LightingAngle](../../aspose.cells.drawing/format3d/lightingangle/) { get; set; } | Obtient et définit l'angle d'éclairage. Plage de 0 à 359,9 degrés. |
| [SurfaceLightingType](../../aspose.cells.drawing/format3d/surfacelightingtype/) { get; set; } | Obtient et définit le type d'éclairage qui doit être appliqué à la scène de la forme. La valeur par défaut est LightRigType.ThreePoint. |
| [SurfaceMaterialType](../../aspose.cells.drawing/format3d/surfacematerialtype/) { get; set; } | Obtient et définit le type de matériau qui est combiné aux propriétés d'éclairage pour donner l'apparence finale d'une forme. La valeur par défaut est PresetMaterialType.WarmMatte. |
| [TopBevel](../../aspose.cells.drawing/format3d/topbevel/) { get; } | Obtient l'objet [`Bevel`](../bevel/) qui contient les propriétés associées à la définition d'un chanfrein sur la face supérieure ou avant d'une forme. |

## Méthodes

| Nom | Description |
| --- | --- |
| [HasTopBevelData](../../aspose.cells.drawing/format3d/hastopbeveldata/)() | Indique si la forme possède des données de chanfrein supérieur |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class Format3DDemo
    {
        public static void RunDemo()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = sheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Ajouter des séries au graphique
            chart.NSeries.Add("A1:A4", true);

            // Accéder à la première série
            Series series = chart.NSeries[0];

            // Accéder au format 3D de la série
            Format3D format3D = series.ShapeProperties.Format3D;

            // Définir les propriétés du format 3D
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Vérifier si la forme possède des données de chanfrein supérieur
            if (format3D.HasTopBevelData())
            {
                Bevel topBevel = format3D.TopBevel;
                Console.WriteLine("Top Bevel Width: " + topBevel.Width);
                Console.WriteLine("Top Bevel Height: " + topBevel.Height);
            }

            // Enregistrez le classeur
            workbook.Save("Format3DDemo.xlsx");
            workbook.Save("Format3DDemo.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


