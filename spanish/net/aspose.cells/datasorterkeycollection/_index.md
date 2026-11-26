---
title: "Clase DataSorterKeyCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.DataSorterKeyCollection. Representa la lista de claves del clasificador de datos"
type: docs
url: /es/net/aspose.cells/datasorterkeycollection/
---
## DataSorterKeyCollection class

Representa la lista de claves del ordenador de datos.

```csharp
public class DataSorterKeyCollection : CollectionBase<DataSorterKey>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [DataSorterKeyCollection](datasorterkeycollection/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/datasorterkeycollection/item/) { get; } | Obtiene y establece [`DataSorterKey`](../datasorterkey/) por índice. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DataSorterKey) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DataSorterKey, IComparer&lt;DataSorterKey&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DataSorterKey, IComparer&lt;DataSorterKey&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DataSorterKey) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DataSorterKey[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DataSorterKey[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, DataSorterKey[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;DataSorterKey&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;DataSorterKey&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;DataSorterKey&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;DataSorterKey&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;DataSorterKey&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;DataSorterKey&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataSorterKey) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataSorterKey, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataSorterKey, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataSorterKey) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataSorterKey, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataSorterKey, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyCollectionDemo
    {
        public static void DataSorterKeyCollectionExample()
        {
            // Instanciar un nuevo objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(80);

            // Obtenga el objeto DataSorter del libro de trabajo
            DataSorter sorter = workbook.DataSorter;

            // Establezca el primer orden para el objeto DataSorter
            sorter.Order1 = Aspose.Cells.SortOrder.Descending;
            // Definir la primera clave
            sorter.Key1 = 1; // Sorting by the second column (Score)

            // Crear un área de celdas (rango)
            CellArea ca = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // Ordene los datos en el rango de datos especificado (A2:B4)
            sorter.Sort(worksheet.Cells, ca);

            // Acceda a DataSorterKeyCollection
            DataSorterKeyCollection keys = sorter.Keys;

            // Muestre el recuento de claves
            Console.WriteLine("Number of keys: " + keys.Count);

            // Acceda a la primera clave y muestre sus propiedades
            DataSorterKey key = keys[0];
            Console.WriteLine("Key Index: " + key.Index);
            Console.WriteLine("Key Order: " + key.Order);

            // Guarda el libro de trabajo
            workbook.Save("DataSorterKeyCollectionExample.xlsx");
            workbook.Save("DataSorterKeyCollectionExample.pdf");
            return;
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [DataSorterKey](../datasorterkey/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


