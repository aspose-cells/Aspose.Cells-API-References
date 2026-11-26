---
title: "Class ChartCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.ChartCollection class. Encapsula una colección de objetos Chart"
type: docs
url: /es/net/aspose.cells.charts/chartcollection/
---
## ChartCollection class

Encapsula una colección de objetos [`Chart`](../chart/).

```csharp
public class ChartCollection : CollectionBase<Chart>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/chartcollection/item/) { get; } | Obtiene el elemento [`Chart`](../chart/) en el índice especificado. (2 indexadores) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.charts/chartcollection/add/#add)(ChartType, int, int, int, int) | Añade un gráfico a la colección. |
| [Add](../../aspose.cells.charts/chartcollection/add/#add_2)(ChartType, string, int, int, int, int) | (**Obsolete.**) Añade un gráfico a la colección. |
| [Add](../../aspose.cells.charts/chartcollection/add/#add_3)(byte[], string, bool, int, int, int, int) | Añade un gráfico con una plantilla predefinida. |
| [Add](../../aspose.cells.charts/chartcollection/add/#add_1)(ChartType, string, bool, int, int, int, int) | Añade un gráfico a la colección. |
| [AddFloatingChart](../../aspose.cells.charts/chartcollection/addfloatingchart/)(ChartType, int, int, int, int) | Añade un gráfico a la colección. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Chart) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Chart, IComparer&lt;Chart&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Chart, IComparer&lt;Chart&gt;) |  |
| [Clear](../../aspose.cells.charts/chartcollection/clear/#clear)() | Borra todos los gráficos. (2 métodos) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Chart) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Chart[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Chart[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Chart[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Chart&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Chart&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Chart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Chart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Chart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Chart&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Chart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Chart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Chart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Chart&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Chart) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Chart, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Chart, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Chart) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Chart, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Chart, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/chartcollection/removeat/#removeat)(int) | Elimina un gráfico en el índice específico. (2 métodos) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionDemo
    {
        public static void ChartCollectionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Acceder a la colección de gráficos de la hoja de cálculo
            ChartCollection charts = worksheet.Charts;

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = charts[chartIndex];

            // Establecer el rango de datos para el gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Personalizar el gráfico
            chart.Title.Text = "Sample Chart";
            chart.ShowLegend = true;

            // Guarda el libro de trabajo
            workbook.Save("ChartCollectionExample.xlsx");
            workbook.Save("ChartCollectionExample.pdf");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Chart](../chart/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


