---
title: "Clase HyperlinkCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.HyperlinkCollection. Encapsula una colección de objetos Hyperlink"
type: docs
url: /es/net/aspose.cells/hyperlinkcollection/
---
## HyperlinkCollection class

Encapsula una colección de objetos [`Hyperlink`](../hyperlink/).

```csharp
public class HyperlinkCollection : CollectionBase<Hyperlink>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/hyperlinkcollection/item/) { get; } | Obtiene el elemento [`Hyperlink`](../hyperlink/) en el índice especificado. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_1)(string, int, int, string) | Agrega un hipervínculo a una celda especificada o a un rango de celdas. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add)(int, int, int, int, string) | Agrega un hipervínculo a una celda especificada o a un rango de celdas. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_2)(string, string, string, string, string) | Agrega un hipervínculo a una celda especificada o a un rango de celdas. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [Clear](../../aspose.cells/hyperlinkcollection/clear/#clear)() | Borra todos los hipervínculos. (2 métodos) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Hyperlink) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Hyperlink[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Hyperlink[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Hyperlink[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Hyperlink&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink, int, int) |  |
| [RemoveAt](../../aspose.cells/hyperlinkcollection/removeat/#removeat)(int) | Elimina el hipervínculo en el índice especificado de esta colección. (2 métodos) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkCollectionDemo
    {
        public static void HyperlinkCollectionExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener colección de hipervínculos
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Agregar un hipervínculo a una URL en la celda "A1"
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Agregar otro hipervínculo a una URL en la celda "B1"
            hyperlinks.Add("B1", 1, 1, "http://www.example.com");

            // Agregar un hipervínculo con un rango de celdas
            hyperlinks.Add("C1", 1, 2, "http://www.test.com");

            // Agregar un hipervínculo con un texto específico para mostrar y texto de pantalla
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            // Eliminar el primer hipervínculo
            hyperlinks.RemoveAt(0);

            // Borrar todos los hipervínculos
            hyperlinks.Clear();

            // Agregar un hipervínculo nuevamente para demostrar el guardado
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Guardando el archivo Excel
            workbook.Save("HyperlinkCollectionExample.xlsx");
            workbook.Save("HyperlinkCollectionExample.pdf");
            return;
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


