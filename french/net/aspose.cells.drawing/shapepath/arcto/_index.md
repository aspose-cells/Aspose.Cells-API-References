---
title: "ShapePath.ArcTo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapePath. Ajoute un arc elliptique à la figure actuelle. Le point de départ est le point final de la figure actuelle"
type: docs
url: /fr/net/aspose.cells.drawing/shapepath/arcto/
---
## ShapePath.ArcTo method

Ajoute un arc elliptique à la figure actuelle. Le point de départ est le point final de la figure actuelle.

```csharp
public void ArcTo(float wR, float hR, float stAng, float swAng)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| wR | Single | La demi-largeur de la zone rectangulaire de l'ellipse qui trace l'arc (Unité : Pixel). |
| hR | Single | La demi-hauteur de la zone rectangulaire de l'ellipse qui trace l'arc (Unité : Pixel). |
| stAng | Single | L'angle de départ de l'arc, mesuré en degrés dans le sens horaire à partir de l'axe x (Unité : Degré). Cet angle spécifiera quel angle le long du chemin circulaire supposé sera utilisé comme position de départ pour tracer l'arc. Cet angle de départ sera verrouillé à la dernière position connue du crayon dans le chemin ShapePath. Garantissant ainsi un chemin continu. |
| swAng | Single | L'angle d'oscillation pour un arc. Cet angle spécifiera jusqu'où, en termes d'angle, le long du chemin circulaire supposé l'arc sera prolongé. L'extension à partir de l'angle de départ sera toujours dans le sens horaire autour du cercle supposé (Unité : Degré). |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodArcToWithSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            //Créer un nouveau chemin de forme
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);

            //Créer un nouveau chemin de forme
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                        96.5f, -7.148871f,
                        130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                        182.24997f, 75.351f,
                        201, 120.517795f);
            shapePath1.MoveTo(150, 70);
            shapePath1.ArcTo(25, 25, 0, 270);

            Workbook workbook = new Workbook();

            //ajouter une forme libre
            workbook.Worksheets[0].Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath, shapePath1 });

            // Enregistrer le résultat
            workbook.Save("ShapePathMethodArcToDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


