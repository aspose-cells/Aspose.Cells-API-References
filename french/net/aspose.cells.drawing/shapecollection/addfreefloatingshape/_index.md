---
title: "ShapeCollection.AddFreeFloatingShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une forme flottante libre à la feuille de calcul. S'applique uniquement aux formes ligne/image"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addfreefloatingshape/
---
## ShapeCollection.AddFreeFloatingShape method

Ajoute une forme libre flottante à la feuille de calcul. S'applique uniquement aux formes ligne/image.

```csharp
public Shape AddFreeFloatingShape(MsoDrawingType type, int top, int left, int height, int width, 
    byte[] imageData, bool isOriginalSize)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | Le type de forme. |
| haut | Int32 | Représente le décalage vertical de la forme par rapport à la première ligne de la feuille de calcul, en pixels. |
| gauche | Int32 | Représente le décalage horizontal de la forme par rapport à la première colonne de la feuille de calcul, en pixels. |
| hauteur | Int32 | Représente la hauteur de LineShape, en unité de pixel. |
| largeur | Int32 | Représente la largeur de LineShape, en unité de pixel. |
| imageData | Byte[] | Les données d'image, ne s'appliquent qu'à picture. |
| isOriginalSize | Boolean | Indique si la forme utilise la taille originale lorsque la forme est une image. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeFloatingShapeWithMsoDrawingTypeInt32Int32Int32IDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Ajouter une forme de ligne
            Shape floatingShape_Line = shapes.AddFreeFloatingShape(
                MsoDrawingType.Line, 
                100, 100, 100, 50, 
                null, 
                false);

            // Ajouter une forme image (en utilisant des données d'image d'exemple)
            byte[] imageData = null;
            try
            {
                using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
                {
                    imageData = new byte[fs.Length];
                    fs.Read(imageData, 0, (int)fs.Length);
                }
            }
            catch
            {
                // Créer des données d'image factices si le fichier n'est pas trouvé
                imageData = new byte[100];
            }

            Shape floatingShape_Picture = shapes.AddFreeFloatingShape(
                MsoDrawingType.Picture, 
                200, 100, 100, 50, 
                imageData, 
                false);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


