---
title: "Classe ShapePath"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.ShapePath. Représente un chemin de création composé d'une série de déplacements, lignes et courbes qui, une fois combinés, formeront une forme géométrique"
type: docs
url: /fr/net/aspose.cells.drawing/shapepath/
---
## ShapePath class

Représente un chemin de création composé d'une série de déplacements, de lignes et de courbes qui, une fois combinés, formeront une forme géométrique.

```csharp
public class ShapePath
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ShapePath](shapepath/)() | Initialise une nouvelle instance de la classe `ShapePath`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [HeightPixel](../../aspose.cells.drawing/shapepath/heightpixel/) { get; set; } | Obtient la hauteur de ce chemin en unités de pixels. |
| [PathSegementList](../../aspose.cells.drawing/shapepath/pathsegementlist/) { get; } | (**Obsolète.**) Obtient la liste [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) |
| [PathSegments](../../aspose.cells.drawing/shapepath/pathsegments/) { get; } | Obtient la liste [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) |
| [WidthPixel](../../aspose.cells.drawing/shapepath/widthpixel/) { get; set; } | Obtient la largeur de ce chemin en unités de pixels. |

## Méthodes

| Nom | Description |
| --- | --- |
| [ArcTo](../../aspose.cells.drawing/shapepath/arcto/)(float, float, float, float) | Ajoute un arc elliptique à la figure actuelle. Le point de départ est le point final de la figure actuelle. |
| [Close](../../aspose.cells.drawing/shapepath/close/)() | Ferme la figure actuelle et démarre une nouvelle figure. Si la figure actuelle contient une séquence de lignes et de courbes connectées, la méthode ferme la boucle en reliant une ligne du point final au point de départ. |
| [CubicBezierTo](../../aspose.cells.drawing/shapepath/cubicbezierto/)(float, float, float, float, float, float) | Ajoute une courbe cubique de Bézier à la figure actuelle. Le point de départ est le point final de la figure actuelle. Unité : Pixel. |
| [LineTo](../../aspose.cells.drawing/shapepath/lineto/)(float, float) | Ajoute un segment de ligne à la figure actuelle. Le point de départ est le point final de la figure actuelle. Unité : Pixel. |
| [MoveTo](../../aspose.cells.drawing/shapepath/moveto/)(float, float) | Démarre une nouvelle figure à partir du point spécifié sans fermer la figure actuelle. Tous les points suivants ajoutés au chemin sont ajoutés à cette nouvelle figure. Unité : Pixel. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePathDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme personnalisée avec tous les paramètres requis
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            
            // Accédez à la ShapePathCollection
            ShapePathCollection shapePaths = customShape.Paths;

            // Ajoutez un nouveau chemin et accédez-y
            int pathIndex = shapePaths.Add();
            ShapePath newPath = shapePaths[pathIndex];

            // Affiche le nombre de chemins
            Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count.ToString());

            // Enregistrez le classeur
            workbook.Save("ShapePathDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


