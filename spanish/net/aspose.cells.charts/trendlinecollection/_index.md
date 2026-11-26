---
title: "Clase TrendlineCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.TrendlineCollection. Representa una colección de todos los objetos Trendline para la serie de datos especificada"
type: docs
url: /es/net/aspose.cells.charts/trendlinecollection/
---
## TrendlineCollection class

Representa una colección de todos los objetos [`Trendline`](../trendline/) para la serie de datos especificada.

```csharp
public class TrendlineCollection : CollectionBase<Trendline>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/trendlinecollection/item/) { get; } | Obtiene un objeto [`Trendline`](../trendline/) por su índice. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.charts/trendlinecollection/add/#add)(TrendlineType) | Agrega un objeto [`Trendline`](../trendline/) a esta colección con el tipo especificado. |
| [Add](../../aspose.cells.charts/trendlinecollection/add/#add_1)(TrendlineType, string) | Agrega un objeto [`Trendline`](../trendline/) a esta colección con el tipo y nombre especificados. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Trendline) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Trendline, IComparer&lt;Trendline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Trendline, IComparer&lt;Trendline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Trendline) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Trendline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Trendline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Trendline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Trendline&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Trendline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Trendline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Trendline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Trendline) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Trendline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Trendline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Trendline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Trendline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Trendline, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TrendlineCollectionDemo
    {
        public static void TrendlineCollectionExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            
            // Añadiendo una nueva hoja de cálculo al objeto Excel
            int sheetIndex = workbook.Worksheets.Add();
            
            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Agregar valores de muestra a celdas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            
            // Agregar NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B4"
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);
            
            // Agregar una línea de tendencia a la primera serie
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Configurando propiedades de la línea de tendencia
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            trendline.Color = Color.Red;

            // Guardando el archivo Excel
            workbook.Save("TrendlineCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Trendline](../trendline/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


