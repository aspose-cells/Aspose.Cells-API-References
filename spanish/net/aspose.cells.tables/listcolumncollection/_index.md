---
title: "Clase ListColumnCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Tables.ListColumnCollection. Representa una lista de todos los objetos ListColumn en la tabla"
type: docs
url: /es/net/aspose.cells.tables/listcolumncollection/
---
## ListColumnCollection class

Representa una lista de todos los objetos [`ListColumn`](../listcolumn/) en la tabla.

```csharp
public class ListColumnCollection : CollectionBase<ListColumn>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/listcolumncollection/item/) { get; } | Obtiene el ListColumn por el índice. (2 indexadores) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListColumn) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListColumn, IComparer&lt;ListColumn&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ListColumn, IComparer&lt;ListColumn&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ListColumn) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListColumn[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListColumn[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ListColumn[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ListColumn&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ListColumn&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ListColumn&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ListColumn&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn, int, int) |  |
| [RemoveAt](../../aspose.cells.tables/listcolumncollection/removeat/#removeat)(int) | Elimina [`ListColumn`](../listcolumn/) por índice. (2 métodos) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnCollectionDemo
    {
        public static void ListColumnCollectionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Poblar la hoja de cálculo con algunos datos
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Agregar un ListObject (tabla) a la hoja de cálculo
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Accede a la ListColumnCollection del ListObject
            ListColumnCollection listColumns = table.ListColumns;

            // Demuestra el acceso a las propiedades de ListColumnCollection
            Console.WriteLine("Number of columns in the table: " + listColumns.Count);

            // Accede a un ListColumn individual por índice
            ListColumn firstColumn = listColumns[0];
            Console.WriteLine("First column name: " + firstColumn.Name);

            // Modifica la capacidad de la ListColumnCollection
            listColumns.Capacity = 10;
            Console.WriteLine("New capacity of the ListColumnCollection: " + listColumns.Capacity);

            // Guarda el libro de trabajo
            workbook.Save("ListColumnCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ListColumn](../listcolumn/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


