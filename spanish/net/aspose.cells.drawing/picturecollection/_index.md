---
title: "Clase PictureCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.PictureCollection. Encapsula una colección de objetos Picture"
type: docs
url: /es/net/aspose.cells.drawing/picturecollection/
---
## PictureCollection class

Encapsula una colección de objetos [`Picture`](../picture/).

```csharp
public class PictureCollection : CollectionBase<Picture>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/picturecollection/item/) { get; } | Obtiene el elemento [`Picture`](../picture/) en el índice especificado. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_2)(int, int, Stream) | Agrega una picture a la colección. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_4)(int, int, string) | Agrega una picture a la colección. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add)(int, int, int, int, Stream) | Agrega una picture a la colección. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_1)(int, int, int, int, string) | Agrega una picture a la colección. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_3)(int, int, Stream, int, int) | Agrega una picture a la colección. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_5)(int, int, string, int, int) | Agrega una picture a la colección. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Picture) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Picture, IComparer&lt;Picture&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Picture, IComparer&lt;Picture&gt;) |  |
| [Camera](../../aspose.cells.drawing/picturecollection/camera/)(int, int, string) | Toma una foto del rango. |
| [Clear](../../aspose.cells.drawing/picturecollection/clear/#clear)() | Borrar todas las imágenes. (2 métodos) |
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
| [RemoveAt](../../aspose.cells.drawing/picturecollection/removeat/#removeat)(int) | Eliminar formas en el índice específico (2 métodos) |

### Ejemplos

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
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Accediendo a la primera hoja de cálculo en el libro de trabajo
            Worksheet worksheet = workbook.Worksheets[0];

            // Accediendo a la PictureCollection de la hoja de cálculo
            PictureCollection pictures = worksheet.Pictures;

            // Añadiendo una imagen usando una ruta de archivo
            int pictureIndex1 = pictures.Add(1, 1, 5, 5, "PictureCollectionExample.jpg");

            // Añadiendo una imagen usando un flujo
            using (FileStream stream = new FileStream("PictureCollectionExample2.jpg", FileMode.Open))
            {
                int pictureIndex2 = pictures.Add(6, 1, 10, 5, stream);
            }

            // Añadiendo una imagen con escalado
            int pictureIndex3 = pictures.Add(11, 1, "PictureCollectionExample3.jpg", 50, 50);

            // Accediendo a una imagen de la colección
            Picture picture = pictures[pictureIndex1];

            // Modificando las propiedades de la imagen
            picture.Left = 10;
            picture.Top = 10;

            // Borrando todas las imágenes de la colección
            pictures.Clear();

            // Guardando el libro de trabajo
            workbook.Save("PictureCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Picture](../picture/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


