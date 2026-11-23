---
title: "Classe Floor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.Floor. Encapsule l'objet qui représente le plancher d'un graphique 3D."
type: docs
url: /fr/net/aspose.cells.charts/floor/
---
## Floor class

Encapsule l'objet qui représente le plancher d'un graphique 3D.

```csharp
public class Floor : Area
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Obtient ou définit la couleur d'arrière-plan du [`Area`](../../aspose.cells.drawing/area/).(Hérité de [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Obtient ou définit la bordure du [`Line`](../../aspose.cells.drawing/line/). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Représente un objet [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) qui contient les propriétés de format de remplissage pour le graphique ou la forme spécifié(e).(Hérité de [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Obtient ou définit la couleur de premier plan.(Hérité de [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Représente le formatage de la zone.(Hérité de [`Area`](../../aspose.cells.drawing/area/).) |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Si la propriété est vraie et que la valeur du point du graphique est un nombre négatif, la couleur de premier plan et la couleur d'arrière-plan seront échangées.(Hérité de [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Renvoie ou définit le degré de transparence de la zone comme une valeur de 0.0 (opaque) à 1.0 (transparent).(Hérité de [`Area`](../../aspose.cells.drawing/area/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FloorDemo
    {
        public static void FloorExample()
        {
            // Instancier l'objet classeur
            Workbook workbook = new Workbook();

            // Obtenir la collection de cellules
            Cells cells = workbook.Worksheets[0].Cells;

            // Insérer des valeurs dans les cellules
            cells["A1"].PutValue(1);
            cells["A2"].PutValue(2);
            cells["A3"].PutValue(3);

            // Obtenir la collection de graphiques
            ChartCollection charts = workbook.Worksheets[0].Charts;

            // Ajouter un nouveau graphique
            int index = charts.Add(ChartType.Column3DStacked, 5, 0, 15, 5);

            // Obtenir le graphique nouvellement ajouté
            Chart chart = charts[index];

            // Définir nseries du graphique
            chart.NSeries.Add("A1:A3", true);

            // Afficher les étiquettes de données
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Obtenir le plan du graphique
            Floor floor = chart.Floor;

            // Définir la bordure du plan en rouge
            floor.Border.Color = Color.Red;

            // Définir le format de remplissage
            floor.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);

            // Définir des propriétés supplémentaires
            floor.BackgroundColor = Color.LightBlue;
            floor.ForegroundColor = Color.DarkBlue;
            floor.Formatting = FormattingType.Custom;
            floor.InvertIfNegative = true;
            floor.Transparency = 0.5;

            // Enregistrer le fichier
            workbook.Save(@"FloorExample.xlsx");
            workbook.Save(@"FloorExample.pdf");
        }
    }
}
```

### Voir aussi

* class [Area](../../aspose.cells.drawing/area/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


