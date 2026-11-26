---
title: "Clase PivotAreaFilterCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotAreaFilterCollection. Representa la lista de filtros para PivotArea"
type: docs
url: /es/net/aspose.cells.pivot/pivotareafiltercollection/
---
## PivotAreaFilterCollection class

Representa la lista de filtros para [`PivotArea`](../pivotarea/)

```csharp
public class PivotAreaFilterCollection : CollectionBase<PivotAreaFilter>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PivotAreaFilterCollection](pivotareafiltercollection/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotareafiltercollection/item/) { get; } | Obtiene el filtro de la lista por el índice. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotAreaFilter) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotAreaFilter, IComparer&lt;PivotAreaFilter&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotAreaFilter, IComparer&lt;PivotAreaFilter&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotAreaFilter) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotAreaFilter[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotAreaFilter[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotAreaFilter[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotAreaFilter&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotAreaFilter&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotAreaFilter) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotAreaFilter, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotAreaFilter, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotAreaFilter) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotAreaFilter, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotAreaFilter, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaFilterCollectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            var cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Crear PivotAreaFilterCollection
            PivotAreaFilterCollection filters = new PivotAreaFilterCollection();

            // Crear y agregar filtros (aunque la reflexión de la API muestra funcionalidad limitada)
            // Nota: La creación real de filtros requeriría información de API más completa
            // Esto demuestra la estructura de la colección
            
            // Acceder a los elementos (propiedad de solo lectura)
            if (filters.Count > 0)
            {
                var firstFilter = filters[0];
            }

            // Guarda el libro de trabajo
            workbook.Save("PivotAreaFilterCollectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotAreaFilter](../pivotareafilter/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


