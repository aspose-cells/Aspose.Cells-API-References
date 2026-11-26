---
title: "Class HorizontalPageBreakCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.HorizontalPageBreakCollection class. Encapsula una colección de objetos HorizontalPageBreak"
type: docs
url: /es/net/aspose.cells/horizontalpagebreakcollection/
---
## HorizontalPageBreakCollection class

Encapsula una colección de objetos [`HorizontalPageBreak`](../horizontalpagebreak/).

```csharp
public class HorizontalPageBreakCollection : CollectionBase<HorizontalPageBreak>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/horizontalpagebreakcollection/item/) { get; } | Obtiene el elemento [`HorizontalPageBreak`](../horizontalpagebreak/) en el índice especificado. (2 indexadores) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add)(int) | Agrega un salto de página horizontal a la colección. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_3)(string) | Agrega un salto de página horizontal a la colección. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_1)(int, int) | Agrega un salto de página horizontal a la colección. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_2)(int, int, int) | Agrega un salto de página horizontal a la colección. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HorizontalPageBreak) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HorizontalPageBreak, IComparer&lt;HorizontalPageBreak&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HorizontalPageBreak, IComparer&lt;HorizontalPageBreak&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HorizontalPageBreak) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HorizontalPageBreak[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HorizontalPageBreak[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HorizontalPageBreak[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak, int, int) |  |
| [RemoveAt](../../aspose.cells/horizontalpagebreakcollection/removeat/#removeat)(int) | Elimina el elemento HPageBreak con un nombre especificado. (2 métodos) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakCollectionDemo
    {
        public static void HorizontalPageBreakCollectionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un salto de página horizontal en la fila 5
            worksheet.HorizontalPageBreaks.Add(5);
            
            // Agregar un salto de página horizontal en la fila 10, comenzando desde la columna 1 hasta la columna 5
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            // Agregar un salto de página horizontal en la fila 15, comenzando desde la columna 2
            worksheet.HorizontalPageBreaks.Add(15, 2);
            
            // Agregar un salto de página horizontal en la celda "G5"
            worksheet.HorizontalPageBreaks.Add("G5");
            
            // Eliminar el primer salto de página horizontal
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            // Guarda el libro de trabajo
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
            workbook.Save("HorizontalPageBreakCollectionExample.pdf");
            return;
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HorizontalPageBreak](../horizontalpagebreak/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


