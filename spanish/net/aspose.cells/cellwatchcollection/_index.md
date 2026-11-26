---
title: "Clase CellWatchCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.CellWatchCollection clase. Representa la colección de celdas en esta hoja de cálculo que se están observando en la ventana de vigilancia"
type: docs
url: /es/net/aspose.cells/cellwatchcollection/
---
## CellWatchCollection class

Representa la colección de celdas de esta hoja de cálculo que se están observando en la 'ventana de observación'.

```csharp
public class CellWatchCollection : CollectionBase<CellWatch>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CellWatchCollection](cellwatchcollection/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/cellwatchcollection/item/) { get; } | Obtiene y establece [`CellWatch`](../cellwatch/) por índice. (2 indexadores) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/cellwatchcollection/add/#add_1)(string) | Agrega [`CellWatch`](../cellwatch/) con el nombre de la celda. |
| [Add](../../aspose.cells/cellwatchcollection/add/#add)(int, int) | Agrega [`CellWatch`](../cellwatch/) con una fila y una columna. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CellWatch) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CellWatch) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CellWatch[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CellWatch[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CellWatch[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CellWatch&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CellWatch&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionDemo
    {
        public static void CellWatchCollectionExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            
            // Obtener la primera Worksheet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Añadir elemento de vigilancia de celda a la ventana de observación
            int watchIndex = sheet.CellWatches.Add("B2");
            
            // Acceder a la CellWatchCollection
            CellWatchCollection cellWatches = sheet.CellWatches;
            
            // Acceder al elemento CellWatch añadido
            CellWatch cellWatch = cellWatches[watchIndex];
            
            // Mostrar las propiedades del elemento CellWatch
            Console.WriteLine("Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            // Modificar las propiedades del elemento CellWatch
            cellWatch.Row = 1;
            cellWatch.Column = 1;
            cellWatch.CellName = "A2";
            
            // Mostrar las propiedades modificadas del elemento CellWatch
            Console.WriteLine("Modified Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            // Guarda el libro de trabajo
            workbook.Save("CellWatchCollectionExample.xlsx");
            workbook.Save("CellWatchCollectionExample.pdf");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [CellWatch](../cellwatch/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


