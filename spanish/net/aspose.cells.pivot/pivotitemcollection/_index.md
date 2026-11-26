---
title: "Clase PivotItemCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotItemCollection. Representa todos los objetos PivotItem en el PivotField"
type: docs
url: /es/net/aspose.cells.pivot/pivotitemcollection/
---
## PivotItemCollection class

Representa todos los objetos [`PivotItem`](../pivotitem/) en el PivotField.

```csharp
public class PivotItemCollection : CollectionBase<PivotItem>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotitemcollection/item/) { get; } | Obtiene el objeto PivotItem en el índice específico. (2 indexadores) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotItem) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotItem, IComparer&lt;PivotItem&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotItem, IComparer&lt;PivotItem&gt;) |  |
| [ChangeitemsOrder](../../aspose.cells.pivot/pivotitemcollection/changeitemsorder/)(int, int) | (**Obsolete.**) Cambia directamente el orden de los dos elementos. |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotItem) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotItem[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotItem[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotItem[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotItem&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotItem&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotItem&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotItem&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [HideAllDetail](../../aspose.cells.pivot/pivotitemcollection/hidealldetail/)(bool) | (**Obsolete.**) Establece si se oculta todo el detalle de todos los PivotItems en un campo pivot. Es decir, colapsar/expandir este campo. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotItem) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotItem, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotItem, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotItem) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotItem, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotItem, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [SwapItem](../../aspose.cells.pivot/pivotitemcollection/swapitem/)(int, int) | Intercambia directamente dos elementos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemCollectionDemo
    {
        public static void PivotItemCollectionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[4, 0].Value = "Date";

            worksheet.Cells[0, 1].Value = "Quantity";
            worksheet.Cells[1, 1].Value = 10;
            worksheet.Cells[2, 1].Value = 20;
            worksheet.Cells[3, 1].Value = 30;
            worksheet.Cells[4, 1].Value = 40;

            // Agregar una tabla dinámica a la hoja de cálculo
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity

            // Accede al PivotField y sus PivotItems
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            // Muestra el recuento de elementos pivot
            Console.WriteLine("Pivot Items Count: " + pivotItems.Count);

            // Itera a través de los elementos pivot y muestra sus nombres
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine("Pivot Item: " + item.Name);
            }

            // Cambia el orden de los elementos pivot
            pivotItems.ChangeitemsOrder(0, 2);

            // Guarda el libro de trabajo
            workbook.Save("PivotItemCollectionExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotItem](../pivotitem/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


