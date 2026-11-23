---
title: "PictureCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PictureCollection. Supprime les formes à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.drawing/picturecollection/removeat/
---
## PictureCollection.RemoveAt method

Supprime les formes à l'index spécifique

```csharp
public void RemoveAt(int index)
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des images à la feuille de calcul
            int index1 = worksheet.Pictures.Add(1, 1, "image1.png");
            int index2 = worksheet.Pictures.Add(5, 1, "image2.png");
            int index3 = worksheet.Pictures.Add(10, 1, "image3.png");

            Console.WriteLine("Number of pictures before removal: " + worksheet.Pictures.Count);

            // Supprimer l'image à l'index spécifié
            worksheet.Pictures.RemoveAt(index2);

            Console.WriteLine("Number of pictures after removal: " + worksheet.Pictures.Count);
        }
    }
}
```

### Voir aussi

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


