---
title: "Classe ShapePathPoint"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.ShapePathPoint. Spécifiez les coordonnées de position ou les marqueurs d'angle. Les coordonnées de position représentent les coordonnées d'un chemin dans un espace de coordonnées, par ex. X/Y. Les marqueurs d'angle indiquent les changements angulaires d'un chemin, par ex. les angles de départ et d'arc d'une courbe"
type: docs
url: /fr/net/aspose.cells.drawing/shapepathpoint/
---
## ShapePathPoint class

Spécifiez les coordonnées de position ou les repères d'angle. Les coordonnées de position représentent les coordonnées d'un chemin dans un espace de coordonnées (par ex. X/Y). Les repères d'angle indiquent les changements angulaires dans un chemin (par ex. les angles de départ et d'oscillation d'un arc).

```csharp
public class ShapePathPoint
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Type](../../aspose.cells.drawing/shapepathpoint/type/) { get; } | Spécifie le type de valeur de l'objet actuel. |
| [X](../../aspose.cells.drawing/shapepathpoint/x/) { get; set; } | (**Obsolete.**) Obtient et définit la coordonnée x pour cette coordonnée de position. Unité EMUs. |
| [XAngle](../../aspose.cells.drawing/shapepathpoint/xangle/) { get; set; } | Lorsque l'objet est un marqueur d'angle, obtenez ou définissez le premier angle en degrés. |
| [XPixel](../../aspose.cells.drawing/shapepathpoint/xpixel/) { get; set; } | Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée x en pixels. |
| [Y](../../aspose.cells.drawing/shapepathpoint/y/) { get; set; } | (**Obsolete.**) Obtient la coordonnée y pour cette coordonnée de position. Unité EMUs. |
| [YAngle](../../aspose.cells.drawing/shapepathpoint/yangle/) { get; set; } | Lorsque l'objet est un marqueur d'angle, obtenez ou définissez le deuxième angle en degrés. |
| [YPixel](../../aspose.cells.drawing/shapepathpoint/ypixel/) { get; set; } | Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée y en pixels. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Ajouter une forme qui contiendra des points de chemin avec tous les paramètres requis
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 10, 10, 200, 200);
                
                // Obtenir les points de chemin géométriques
                CustomGeometry geometry = shape.Geometry as CustomGeometry;
                if (geometry != null && geometry.Paths.Count > 0)
                {
                    ShapePath path = geometry.Paths[0];
                    
                    // Accéder à un point de chemin existant (si disponible)
                    if (path.PathSegementList.Count > 0)
                    {
                        // Obtenir le premier point (l'implémentation réelle peut varier en fonction du type de segment)
                        ShapePathPoint point = path.PathSegementList[0].Points[0];
                        
                        // Afficher les coordonnées du point
                        Console.WriteLine($"ShapePathPoint at X: {point.X}, Y: {point.Y}");
                    }
                }
                
                // Enregistrez le classeur
                workbook.Save("ShapePathPointDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPoint: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


