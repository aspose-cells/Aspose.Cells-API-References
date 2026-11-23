---
title: "Classe PictureCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.PictureCollection. Encapsule une collection d'objets Picture"
type: docs
url: /fr/net/aspose.cells.drawing/picturecollection/
---
## PictureCollection class

Encapsule une collection de [`Picture`](../picture/) objets.

```csharp
public class PictureCollection : CollectionBase<Picture>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/picturecollection/item/) { get; } | Obtient l'élément [`Picture`](../picture/) à l'index spécifié. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_2)(int, int, Stream) | Ajoute une image à la collection. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_4)(int, int, string) | Ajoute une image à la collection. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add)(int, int, int, int, Stream) | Ajoute une image à la collection. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_1)(int, int, int, int, string) | Ajoute une image à la collection. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_3)(int, int, Stream, int, int) | Ajoute une image à la collection. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_5)(int, int, string, int, int) | Ajoute une image à la collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Picture) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Picture, IComparer&lt;Picture&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Picture, IComparer&lt;Picture&gt;) |  |
| [Camera](../../aspose.cells.drawing/picturecollection/camera/)(int, int, string) | Prend une photo de la plage. |
| [Clear](../../aspose.cells.drawing/picturecollection/clear/#clear)() | Effacer toutes les images. (2 méthodes) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Picture) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Picture[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Picture[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Picture[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Picture&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Picture&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Picture&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Picture&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Picture&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Picture&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Picture&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Picture&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Picture&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Picture&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Picture) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Picture, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Picture, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Picture) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Picture, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Picture, int, int) |  |
| [RemoveAt](../../aspose.cells.drawing/picturecollection/removeat/#removeat)(int) | Supprimer les formes à l'index spécifique (2 méthodes) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PictureCollectionDemo
    {
        public static void PictureCollectionExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Accès à la première feuille de calcul du classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la PictureCollection de la feuille de calcul
            PictureCollection pictures = worksheet.Pictures;

            // Ajouter une image en utilisant un chemin de fichier
            int pictureIndex1 = pictures.Add(1, 1, 5, 5, "PictureCollectionExample.jpg");

            // Ajouter une image en utilisant un flux
            using (FileStream stream = new FileStream("PictureCollectionExample2.jpg", FileMode.Open))
            {
                int pictureIndex2 = pictures.Add(6, 1, 10, 5, stream);
            }

            // Ajouter une image avec mise à l'échelle
            int pictureIndex3 = pictures.Add(11, 1, "PictureCollectionExample3.jpg", 50, 50);

            // Accéder à une image de la collection
            Picture picture = pictures[pictureIndex1];

            // Modifier les propriétés de l'image
            picture.Left = 10;
            picture.Top = 10;

            // Effacer toutes les images de la collection
            pictures.Clear();

            // Enregistrement du classeur
            workbook.Save("PictureCollectionExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Picture](../picture/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


