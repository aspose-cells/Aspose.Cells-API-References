---
title: "Klass PictureCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.PictureCollection-klass. Inkapslar en samling av Picture-objekt"
type: docs
url: /sv/net/aspose.cells.drawing/picturecollection/
---
## PictureCollection class

Inkapslar en samling av [`Picture`](../picture/) objekt.

```csharp
public class PictureCollection : CollectionBase<Picture>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/picturecollection/item/) { get; } | Hämtar [`Picture`](../picture/) elementet på det angivna indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_2)(int, int, Stream) | Lägger till en bild i samlingen. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_4)(int, int, string) | Lägger till en bild i samlingen. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add)(int, int, int, int, Stream) | Lägger till en bild i samlingen. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_1)(int, int, int, int, string) | Lägger till en bild i samlingen. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_3)(int, int, Stream, int, int) | Lägger till en bild i samlingen. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_5)(int, int, string, int, int) | Lägger till en bild i samlingen. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Picture) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Picture, IComparer&lt;Picture&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Picture, IComparer&lt;Picture&gt;) |  |
| [Camera](../../aspose.cells.drawing/picturecollection/camera/)(int, int, string) | Tar ett foto av området. |
| [Clear](../../aspose.cells.drawing/picturecollection/clear/#clear)() | Rensa alla bilder. (2 metoder) |
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
| [RemoveAt](../../aspose.cells.drawing/picturecollection/removeat/#removeat)(int) | Ta bort former på det specifika indexet (2 metoder) |

### Exempel

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
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till PictureCollection i kalkylbladet
            PictureCollection pictures = worksheet.Pictures;

            // Lägga till en bild med en filsökväg
            int pictureIndex1 = pictures.Add(1, 1, 5, 5, "PictureCollectionExample.jpg");

            // Lägga till en bild med en ström
            using (FileStream stream = new FileStream("PictureCollectionExample2.jpg", FileMode.Open))
            {
                int pictureIndex2 = pictures.Add(6, 1, 10, 5, stream);
            }

            // Lägga till en bild med skalning
            int pictureIndex3 = pictures.Add(11, 1, "PictureCollectionExample3.jpg", 50, 50);

            // Åtkomst till en bild från samlingen
            Picture picture = pictures[pictureIndex1];

            // Modifiera bildens egenskaper
            picture.Left = 10;
            picture.Top = 10;

            // Rensa alla bilder från samlingen
            pictures.Clear();

            // Sparar arbetsboken
            workbook.Save("PictureCollectionExample.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Picture](../picture/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


