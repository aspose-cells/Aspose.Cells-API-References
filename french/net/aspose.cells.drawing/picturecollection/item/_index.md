---
title: "PictureCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PictureCollection. Obtient l'élément Picture à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.drawing/picturecollection/item/
---
## PictureCollection indexer

Obtient le [`Picture`](../../picture/) élément à l'index spécifié.

```csharp
public Picture this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir la collection d'images
            PictureCollection pictures = worksheet.Pictures;
            
            // Ajouter une image (remplacez "image.png" par le chemin réel de l'image)
            int index = pictures.Add(1, 1, "image.png");
            
            // Accéder à l'image en utilisant la propriété Item
            Picture pic = pictures[index];
            
            // Démontrer l'utilisation de la propriété Item
            Console.WriteLine($"Picture at index {index} has width: {pic.Width} and height: {pic.Height}");
            
            // Modifier les propriétés de l'image
            pic.Height = 200;
            pic.Width = 300;
            
            // Enregistrez le classeur
            workbook.Save("PictureCollectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Picture](../../picture/)
* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


