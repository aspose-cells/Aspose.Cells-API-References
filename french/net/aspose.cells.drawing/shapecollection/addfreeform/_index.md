---
title: "ShapeCollection.AddFreeform"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une forme libre à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addfreeform/
---
## ShapeCollection.AddFreeform method

Ajoute une forme libre à la feuille de calcul.

```csharp
public Shape AddFreeform(int topRow, int top, int leftColumn, int left, int height, int width, 
    ShapePath[] paths)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical de la forme libre depuis sa ligne de gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal de la forme libre depuis sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | Représente la hauteur de la forme libre, en unité de pixel. |
| largeur | Int32 | Représente la largeur de la forme libre, en unité de pixel. |
| chemins | ShapePath[] | Représente un chemin défini par l'utilisateur |

### Valeur de retour

Une forme libre.

### Remarques

Remarque : La largeur et la hauteur dans les paramètres peuvent être n'importe quelles valeurs entières positives, et non la largeur et la hauteur totales du tableau ShapePath spécifié par ’paths'. La relation entre elles est une relation d'échelle‑remplissage, c'est‑à‑dire que chaque objet ShapePath sera mis à l'échelle en fonction de la largeur et de la hauteur. Ainsi, lorsqu'il y a plusieurs objets dans 'paths', chaque objet ShapePath doit être conçu de manière raisonnable pour répondre aux attentes. Lorsqu'il n'y a qu'un seul objet ShapePath et qu'il n'existe aucune autre exigence, passer la largeur et la hauteur de l'objet comme valeurs de paramètres est une bonne solution.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeformWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Créer des chemins de figures personnalisés
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
            
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                                96.5f, -7.148871f,
                                130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                                182.24997f, 75.351f,
                                201, 120.517795f);
            shapePath1.MoveTo(150, 80);
            shapePath1.ArcTo(25, 25, 0, 270);
            
            // Ajouter une forme libre à la feuille de calcul
            shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath, shapePath1 });

            // Enregistrez le classeur
            workbook.Save("AddFreeformDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../../shape/)
* class [ShapePath](../../shapepath/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


