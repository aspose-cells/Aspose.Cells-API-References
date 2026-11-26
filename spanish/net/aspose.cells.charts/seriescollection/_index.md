---
title: "Clase SeriesCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.SeriesCollection. Encapsula una colección de objetos Series"
type: docs
url: /es/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Encapsula una colección de objetos [`Series`](../series/).

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata/) { get; set; } | Obtiene o establece el rango de valores del eje de categoría. Puede ser un rango de celdas (como "d1:e10") o una secuencia de valores (como "{2,6,8,10}"). |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried/) { get; set; } | Representa si el color de los puntos varía. |
| [Item](../../aspose.cells.charts/seriescollection/item/) { get; } | Obtiene el elemento [`Series`](../series/) en el índice especificado. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata/) { get; set; } | Obtiene o establece el rango de valores del segundo eje de categoría. Puede ser un rango de celdas (como "d1:e10"), o una secuencia de valores (como "{2,6,8,10}"). Solo tiene efecto cuando algunas series se trazaron en el segundo eje. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add/#add)(string, bool) | Agrega la colección [`Series`](../series/) a un gráfico. |
| [Add](../../aspose.cells.charts/seriescollection/add/#add_1)(string, bool, bool) | Agrega la colección [`Series`](../series/) a un gráfico. |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1/)(string, bool) | Agrega la colección [`Series`](../series/) a un gráfico. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeColors](../../aspose.cells.charts/seriescollection/changecolors/)(ChartColorPaletteType) | Establecer paleta monocromática para las series del gráfico. |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder/)(int, int) | (**Obsolete.**) Cambia directamente el orden de las dos series. |
| [Clear](../../aspose.cells.charts/seriescollection/clear/#clear)() | Limpia la colección (2 métodos) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Series) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Series[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Series[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Series[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Series&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Series&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Series&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Series&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder/)(int) | Obtiene el elemento [`Series`](../series/) por orden. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat/#removeat)(int) | Eliminar una serie en el índice específico. (2 métodos) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames/)(int, string, bool) | Establece los nombres de todas las series en el gráfico. |
| [SwapSeries](../../aspose.cells.charts/seriescollection/swapseries/)(int, int) | Cambia directamente el orden de las dos series. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionDemo
    {
        public static void SeriesCollectionExample()
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
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Accediendo a la instancia del gráfico recién agregado
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // Estableciendo la fuente de datos para los datos de categoría de NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Accediendo a la SeriesCollection del gráfico
            SeriesCollection seriesCollection = chart.NSeries;

            // Estableciendo propiedades de la SeriesCollection
            seriesCollection.CategoryData = "C1:C4";
            seriesCollection.SecondCategoryData = "C1:C4";
            seriesCollection.IsColorVaried = true;

            // Accediendo a una serie específica en la SeriesCollection
            Series series = seriesCollection[0];
            
            // Estableciendo propiedades de la serie
            series.Values = "=B1:B4";
            series.Name = "First Series";
            series.Type = ChartType.Line;
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Guardando el archivo Excel
            workbook.Save("SeriesCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Series](../series/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


