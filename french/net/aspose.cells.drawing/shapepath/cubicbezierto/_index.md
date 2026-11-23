---
title: "ShapePath.CubicBezierTo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapePath. Ajoute une courbe Bézier cubique à la figure actuelle. Le point de départ est le point final de la figure actuelle. Unité Pixel"
type: docs
url: /fr/net/aspose.cells.drawing/shapepath/cubicbezierto/
---
## ShapePath.CubicBezierTo method

Ajoute une courbe cubique de Bézier à la figure actuelle. Le point de départ est le point final de la figure actuelle. Unité : Pixel.

```csharp
public void CubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, 
    float endY)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ctrX1 | Single | La coordonnée x du premier point de contrôle de la courbe (Unité : Pixel). |
| ctrY1 | Single | La coordonnée y du premier point de contrôle de la courbe (Unité : Pixel). |
| ctrX2 | Single | La coordonnée x du deuxième point de contrôle de la courbe (Unité : Pixel). |
| ctrY2 | Single | La coordonnée y du deuxième point de contrôle de la courbe (Unité : Pixel). |
| endX | Single | La coordonnée x du point final de la courbe (Unité : Pixel). |
| endY | Single | La coordonnée y du point final de la courbe (Unité : Pixel). |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCubicBezierToWithSingleSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

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


            //ajouter une forme libre
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath1 });

            // Enregistrer le résultat
            workbook.Save("ShapePathMethodCubicBezierToDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


