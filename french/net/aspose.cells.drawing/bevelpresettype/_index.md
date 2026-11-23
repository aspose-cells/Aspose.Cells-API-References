---
title: "Énum BevelPresetType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énum Aspose.Cells.Drawing.BevelPresetType. Représente un préréglage pour un type de biseau qui peut être appliqué à une forme en 3D"
type: docs
url: /fr/net/aspose.cells.drawing/bevelpresettype/
---
## BevelPresetType enumeration

Représente un préréglage pour un type de biseau qui peut être appliqué à une forme en 3D.

```csharp
public enum BevelPresetType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Pas de biseau |
| Angle | `1` | Angle |
| ArtDeco | `2` | Art déco |
| Circle | `3` | Cercle |
| Convex | `4` | Convexe |
| CoolSlant | `5` | Inclinaison cool |
| Cross | `6` | Croix |
| Divot | `7` | Creux |
| HardEdge | `8` | Bord dur |
| RelaxedInset | `9` | Encart détendu |
| Riblet | `10` | Riblet |
| Slope | `11` | Pente |
| SoftRound | `12` | Arrondi doux |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class BevelPresetTypeDemo
    {
        public static void BevelPresetTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            // Accéder au titre du graphique et définir son texte
            chart.Title.Text = "Sample Chart with Bevel";

            // Accéder à la zone de tracé du graphique
            PlotArea plotArea = chart.PlotArea;

            // Accéder aux propriétés de forme de la zone de tracé
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            
            // Accéder aux propriétés du format 3D
            Format3D format3D = shapeProperties.Format3D;

            // Accéder aux propriétés du biseau supérieur
            Bevel topBevel = format3D.TopBevel;

            // Définir le type de biseau sur "Angle"
            topBevel.Type = BevelPresetType.Angle;

            // Définir la largeur et la hauteur du biseau
            topBevel.Width = 10;
            topBevel.Height = 10;

            // Enregistrez le classeur
            workbook.Save("BevelPresetTypeExample.xlsx");
            workbook.Save("BevelPresetTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


