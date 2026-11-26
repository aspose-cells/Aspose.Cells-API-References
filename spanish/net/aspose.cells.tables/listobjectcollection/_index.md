---
title: "Clase ListObjectCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Tables.ListObjectCollection. Representa una colección de objetos ListObject en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.tables/listobjectcollection/
---
## ListObjectCollection class

Representa una colección de objetos [`ListObject`](../listobject/) en la hoja de cálculo.

```csharp
public class ListObjectCollection : CollectionBase<ListObject>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/listobjectcollection/item/) { get; } | Obtiene el ListObject por índice. (2 indexadores) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.tables/listobjectcollection/add/#add_1)(string, string, bool) | Agrega un ListObject a la hoja de cálculo. |
| [Add](../../aspose.cells.tables/listobjectcollection/add/#add)(int, int, int, int, bool) | Agrega un ListObject a la hoja de cálculo. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListObject) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListObject, IComparer&lt;ListObject&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ListObject, IComparer&lt;ListObject&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ListObject) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListObject[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListObject[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ListObject[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ListObject&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ListObject&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ListObject&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ListObject&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ListObject&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ListObject&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ListObject&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ListObject&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ListObject&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ListObject&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListObject) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListObject, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListObject, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListObject) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListObject, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListObject, int, int) |  |
| [RemoveAt](../../aspose.cells.tables/listobjectcollection/removeat/#removeat)(int) | Eliminar [`ListObject`](../listobject/) por índice. (2 métodos) |
| [UpdateColumnName](../../aspose.cells.tables/listobjectcollection/updatecolumnname/)() | Actualizar todos los nombres de columna de las tablas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectCollectionDemo
    {
        public static void ListObjectCollectionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la ListObjectCollection de la hoja de cálculo
            ListObjectCollection listObjects = worksheet.ListObjects;

            // Agregar un ListObject (tabla) a la hoja de cálculo
            int listObjectIndex = listObjects.Add(0, 0, 10, 4, true);
            ListObject listObject = listObjects[listObjectIndex];

            // Establecer el nombre del ListObject
            listObject.DisplayName = "SampleTable";

            // Poblar la tabla con algunos datos
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["D1"].PutValue("Header4");

            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue("Row" + i + "Col1");
                worksheet.Cells[i, 1].PutValue("Row" + i + "Col2");
                worksheet.Cells[i, 2].PutValue("Row" + i + "Col3");
                worksheet.Cells[i, 3].PutValue("Row" + i + "Col4");
            }

            // Actualizar todos los nombres de columna de las tablas
            listObjects.UpdateColumnName();

            // Guarda el libro de trabajo
            workbook.Save("ListObjectCollectionExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ListObject](../listobject/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


