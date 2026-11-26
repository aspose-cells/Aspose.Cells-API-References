---
title: "Clase SparklineGroupCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.SparklineGroupCollection. Encapsula una colección de objetos SparklineGroup"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroupcollection/
---
## SparklineGroupCollection class

Encapsula una colección de objetos [`SparklineGroup`](../sparklinegroup/).

```csharp
public class SparklineGroupCollection : CollectionBase<SparklineGroup>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/sparklinegroupcollection/item/) { get; } | Obtiene el elemento [`SparklineGroup`](../sparklinegroup/) en el índice especificado. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.charts/sparklinegroupcollection/add/#add)(SparklineType) | Agrega un [`SparklineGroup`](../sparklinegroup/) con un [`Sparkline`](../sparkline/) a la colección. |
| [Add](../../aspose.cells.charts/sparklinegroupcollection/add/#add_1)(SparklineType, string, bool, CellArea) | Agrega un [`SparklineGroup`](../sparklinegroup/) con algunos [`Sparkline`](../sparkline/) a la colección. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SparklineGroup) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SparklineGroup, IComparer&lt;SparklineGroup&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, SparklineGroup, IComparer&lt;SparklineGroup&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [ClearSparklineGroups](../../aspose.cells.charts/sparklinegroupcollection/clearsparklinegroups/)(CellArea) | Borra los grupos de sparkline que se superponen a un área de celdas. |
| [ClearSparklines](../../aspose.cells.charts/sparklinegroupcollection/clearsparklines/)(CellArea) | Borra los sparklines que están dentro de un área de celdas. |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(SparklineGroup) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SparklineGroup[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SparklineGroup[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, SparklineGroup[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;SparklineGroup&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;SparklineGroup&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;SparklineGroup&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;SparklineGroup&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;SparklineGroup&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SparklineGroup) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SparklineGroup, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SparklineGroup, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SparklineGroup) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SparklineGroup, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SparklineGroup, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineGroupCollectionDemo
    {
        public static void SparklineGroupCollectionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Define el CellArea para el sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Añade un grupo de sparkline a la hoja de cálculo
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Añade sparklines al grupo
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 5);

            // Personaliza el grupo de sparkline
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;
            group.LineWeight = 1.0;

            // Guarda el libro de trabajo
            workbook.Save("SparklineGroupCollectionExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [SparklineGroup](../sparklinegroup/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


