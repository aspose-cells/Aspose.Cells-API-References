---
title: "Classe Walls"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.Walls. Encapsule l'objet qui représente les parois d'un graphique 3D"
type: docs
url: /fr/net/aspose.cells.charts/walls/
---
## Walls class

Encapsule l'objet qui représente les parois d'un graphique 3D.

```csharp
public class Walls : Floor
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Obtient ou définit la couleur d'arrière-plan du [`Area`](../../aspose.cells.drawing/area/).(Hérité de [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Obtient ou définit la bordure [`Line`](../../aspose.cells.drawing/line/).(Hérité de [`Floor`](../floor/).) |
| [CenterX](../../aspose.cells.charts/walls/centerx/) { get; } | Obtient la coordonnée x du coin inférieur gauche du centre du mur en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate(). |
| [CenterXPx](../../aspose.cells.charts/walls/centerxpx/) { get; } | Obtient la coordonnée x du coin inférieur gauche du centre du mur en unités de pixels après l'appel de la méthode Chart.Calculate(). |
| [CenterY](../../aspose.cells.charts/walls/centery/) { get; } | Obtient la coordonnée y du coin inférieur gauche du centre du mur en unités de 1/4000 de la hauteur du graphique après l'appel de la méthode Chart.Calculate(). |
| [CenterYPx](../../aspose.cells.charts/walls/centerypx/) { get; } | Obtient la coordonnée y du coin inférieur gauche du centre du mur en unités de pixels après l'appel de la méthode Chart.Calculate(). |
| [Depth](../../aspose.cells.charts/walls/depth/) { get; } | Obtient la profondeur avant‑arrière en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate(). |
| [DepthPx](../../aspose.cells.charts/walls/depthpx/) { get; } | Obtient la profondeur de l'avant vers l'arrière en unités de pixels après l'appel de la méthode Chart.Calculate(). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Représente un objet [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) qui contient les propriétés de format de remplissage pour le graphique ou la forme spécifié(e).(Hérité de [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Obtient ou définit la couleur de premier plan.(Hérité de [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Représente le formatage de la zone.(Hérité de [`Area`](../../aspose.cells.drawing/area/).) |
| [Height](../../aspose.cells.charts/walls/height/) { get; } | Obtient la hauteur de haut en bas en unités de 1/4000 de la hauteur du graphique après l'appel de la méthode Chart.Calculate(). |
| [HeightPx](../../aspose.cells.charts/walls/heightpx/) { get; } | Obtient la hauteur de haut en bas en unités de pixels après avoir appelé la méthode Chart.Calculate(). |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Si la propriété est vraie et que la valeur du point du graphique est un nombre négatif, la couleur de premier plan et la couleur d'arrière-plan seront échangées.(Hérité de [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Renvoie ou définit le degré de transparence de la zone comme une valeur de 0.0 (opaque) à 1.0 (transparent).(Hérité de [`Area`](../../aspose.cells.drawing/area/).) |
| [Width](../../aspose.cells.charts/walls/width/) { get; } | Obtient la largeur de gauche à droite en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate(). |
| [WidthPx](../../aspose.cells.charts/walls/widthpx/) { get; } | Obtient la largeur de gauche à droite en unités de pixels après avoir appelé la méthode Chart.Calculate(). |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetCubePointCount](../../aspose.cells.charts/walls/getcubepointcount/)() | Obtient le nombre de points du cube après l'appel de la méthode Chart.Calculate(). |
| [GetCubePointXPx](../../aspose.cells.charts/walls/getcubepointxpx/)(int) | Obtient la coordonnée x du point d'apex du cube des murs après avoir appelé la méthode Chart.Calculate(). Le nombre de points d'apex du cube des murs est huit. |
| [GetCubePointYPx](../../aspose.cells.charts/walls/getcubepointypx/)(int) | Obtient la coordonnée y du point d'apex du cube des murs après l'appel de la méthode Chart.Calculate(). Le nombre de points d'apex du cube des murs est huit. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class WallsDemo
    {
        public static void WallsExample()
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

            // Ajoutez un graphique 3D à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculez le graphique pour mettre à jour ses propriétés
            chart.Calculate();

            // Accédez aux parois du graphique 3D
            Walls walls = chart.Walls;

            // Définissez les propriétés des parois
            walls.BackgroundColor = Color.LightBlue;
            walls.ForegroundColor = Color.DarkBlue;
            walls.Formatting = FormattingType.Custom;
            walls.InvertIfNegative = true;
            walls.Transparency = 0.5;

            // Accédez à la bordure des parois et définissez ses propriétés
            Line border = walls.Border;
            border.Color = Color.Red;
            border.Style = LineType.Solid;

            // Imprimez certaines propriétés des parois
            Console.WriteLine("CenterX: " + walls.CenterX);
            Console.WriteLine("CenterY: " + walls.CenterY);
            Console.WriteLine("Width: " + walls.Width);
            Console.WriteLine("Depth: " + walls.Depth);
            Console.WriteLine("Height: " + walls.Height);
            Console.WriteLine("CenterXPx: " + walls.CenterXPx);
            Console.WriteLine("CenterYPx: " + walls.CenterYPx);
            Console.WriteLine("WidthPx: " + walls.WidthPx);
            Console.WriteLine("DepthPx: " + walls.DepthPx);
            Console.WriteLine("HeightPx: " + walls.HeightPx);

            // Enregistrez le classeur
            workbook.Save("WallsExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Floor](../floor/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


