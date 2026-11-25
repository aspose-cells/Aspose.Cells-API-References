---
title: "Classe PictureCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.PictureCollection. Incapsula una raccolta di oggetti Picture"
type: docs
url: /it/net/aspose.cells.drawing/picturecollection/
---
## PictureCollection class

Incapsula una raccolta di oggetti [`Picture`](../picture/).

```csharp
public class PictureCollection : CollectionBase<Picture>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/picturecollection/item/) { get; } | Ottiene l'elemento [`Picture`](../picture/) all'indice specificato. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_2)(int, int, Stream) | Aggiunge un'immagine alla collezione. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_4)(int, int, string) | Aggiunge un'immagine alla collezione. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add)(int, int, int, int, Stream) | Aggiunge un'immagine alla collezione. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_1)(int, int, int, int, string) | Aggiunge un'immagine alla collezione. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_3)(int, int, Stream, int, int) | Aggiunge un'immagine alla collezione. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_5)(int, int, string, int, int) | Aggiunge un'immagine alla collezione. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Picture) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Picture, IComparer&lt;Picture&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Picture, IComparer&lt;Picture&gt;) |  |
| [Camera](../../aspose.cells.drawing/picturecollection/camera/)(int, int, string) | Cattura una foto dell'intervallo. |
| [Clear](../../aspose.cells.drawing/picturecollection/clear/#clear)() | Cancella tutte le immagini. (2 metodi) |
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
| [RemoveAt](../../aspose.cells.drawing/picturecollection/removeat/#removeat)(int) | Rimuovi le forme all'indice specifico (2 metodi) |

### Esempi

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
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Accesso al primo foglio di lavoro nella cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Accesso alla PictureCollection del foglio di lavoro
            PictureCollection pictures = worksheet.Pictures;

            // Aggiunta di un'immagine usando un percorso file
            int pictureIndex1 = pictures.Add(1, 1, 5, 5, "PictureCollectionExample.jpg");

            // Aggiunta di un'immagine usando uno stream
            using (FileStream stream = new FileStream("PictureCollectionExample2.jpg", FileMode.Open))
            {
                int pictureIndex2 = pictures.Add(6, 1, 10, 5, stream);
            }

            // Aggiunta di un'immagine con ridimensionamento
            int pictureIndex3 = pictures.Add(11, 1, "PictureCollectionExample3.jpg", 50, 50);

            // Accesso a un'immagine dalla collezione
            Picture picture = pictures[pictureIndex1];

            // Modifica delle proprietà dell'immagine
            picture.Left = 10;
            picture.Top = 10;

            // Cancellazione di tutte le immagini dalla collezione
            pictures.Clear();

            // Salvataggio della cartella di lavoro
            workbook.Save("PictureCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Picture](../picture/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


