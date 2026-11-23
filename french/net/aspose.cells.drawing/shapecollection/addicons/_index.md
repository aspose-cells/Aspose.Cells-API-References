---
title: "ShapeCollection.AddIcons"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une image svg"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addicons/
---
## ShapeCollection.AddIcons method

Ajoute une image svg.

```csharp
public Picture AddIcons(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageByteData, byte[] compatibleImageData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical de la forme depuis sa ligne gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Le décalage horizontal de la forme depuis sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | La hauteur de la forme, en unité de pixel. |
| largeur | Int32 | La largeur de la forme, en unité de pixel. |
| imageByteData | Byte[] | Les données d'image en octets. |
| compatibleImageData | Byte[] | Données d'image converties depuis le svg afin d'être compatibles avec Excel 2016 ou les versions antérieures. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddIconsWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Créer un fichier d'icône d'exemple (dans une utilisation réelle, vous utiliseriez un fichier existant)
            string iconPath = "icon.svg";
            File.WriteAllText(iconPath, "<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100'><circle cx='50' cy='50' r='40' fill='red'/></svg>");

            // Ajouter une icône à la feuille de calcul
            using (FileStream fs = new FileStream(iconPath, FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                Picture picture = shapes.AddIcons(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            // Nettoyer (facultatif)
            File.Delete(iconPath);
        }
    }
}
```

### Voir aussi

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


