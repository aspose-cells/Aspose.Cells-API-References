---
title: SeriesCollection
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula una colección deSeries./series objetos.
type: docs
weight: 830
url: /es/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Encapsula una colección de[`Series`](../series) objetos.

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata) { get; set; } | Obtiene o establece el rango de valores del eje de categoría. Puede ser un rango de celdas (como, "d1:e10"), o una secuencia de valores (como, "{2,6,8,10}"). |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried) { get; set; } | Representa si se varía el color de los puntos. |
| [Item](../../aspose.cells.charts/seriescollection/item) { get; } | Obtiene el[`Series`](../series) elemento en el índice especificado. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata) { get; set; } | Obtiene o establece el rango de valores del eje de segunda categoría. Puede ser un rango de celdas (como, "d1:e10"), o una secuencia de valores (como, "{2,6,8,10}"). Solo efectos cuando algunas ASeries se trazan en el segundo eje. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add#add)(string, bool) | Agrega el[`SeriesCollection`](../seriescollection) colección a un gráfico. |
| [Add](../../aspose.cells.charts/seriescollection/add#add_1)(string, bool, bool) | Agrega el[`SeriesCollection`](../seriescollection) colección a un gráfico. |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1)(string, bool) | Agrega el[`SeriesCollection`](../seriescollection) colección a un gráfico. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder)(int, int) | Cambia directamente el orden de las dos series. |
| [Clear](../../aspose.cells.charts/seriescollection/clear#clear)() | Borra la colección (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Series) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Series[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Series[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Series[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Series&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Series&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Series&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Series&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder)(int) | Obtiene el[`Series`](../series) elemento por pedido. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat#removeat)(int) | Eliminar en una serie en el índice específico. (2 methods) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames)(int, string, bool) | Establece el nombre de todas las series del gráfico. |

### Ejemplos

```csharp

[C#]
// Instanciando un objeto Workbook
Workbook workbook = new Workbook();
//Agregar una nueva hoja de cálculo al objeto de Excel
int sheetIndex = workbook.Worksheets.Add();
//Obteniendo la referencia de la hoja de trabajo recién agregada pasando su índice de hoja
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// Agregar un valor de muestra a la celda "A1"
worksheet.Cells["A1"].PutValue(50);
// Agregar un valor de muestra a la celda "A2"
worksheet.Cells["A2"].PutValue(100);
// Agregar un valor de muestra a la celda "A3"
worksheet.Cells["A3"].PutValue(150);
// Agregar un valor de muestra a la celda "A4"
worksheet.Cells["A4"].PutValue(200);
// Agregar un valor de muestra a la celda "B1"
worksheet.Cells["B1"].PutValue(60);
// Agregar un valor de muestra a la celda "B2"
worksheet.Cells["B2"].PutValue(32);
// Agregar un valor de muestra a la celda "B3"
worksheet.Cells["B3"].PutValue(50);
// Agregar un valor de muestra a la celda "B4"
worksheet.Cells["B4"].PutValue(40);
// Agregar un valor de muestra a la celda "C1" como datos de categoría
worksheet.Cells["C1"].PutValue("Q1");
// Agregar un valor de muestra a la celda "C2" como datos de categoría
worksheet.Cells["C2"].PutValue("Q2");
// Agregar un valor de muestra a la celda "C3" como datos de categoría
worksheet.Cells["C3"].PutValue("Y1");
// Agregar un valor de muestra a la celda "C4" como datos de categoría
worksheet.Cells["C4"].PutValue("Y2");
//Añadiendo un gráfico a la hoja de trabajo
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accediendo a la instancia del gráfico recién agregado
Chart chart = worksheet.Charts[chartIndex];
// Agregar NSeries (fuente de datos del gráfico) al gráfico que va desde la celda "A1" hasta la celda "B4"
chart.NSeries.Add("A1:B4", true);
//Configuración de la fuente de datos para la categoría de datos de NSeries
chart.NSeries.CategoryData = "C1:C4";
//Guardando el archivo de Excel
workbook.Save("book1.xls");

[Visual Basic]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()
'Agregar una nueva hoja de cálculo al objeto de Excel
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'Obtener la referencia de la hoja de trabajo recién agregada pasando su índice de hoja
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Adición de un gráfico a la hoja de cálculo
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Acceso a la instancia del gráfico recién agregado
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'Configuración de la fuente de datos para los datos de categoría de NSeries
chart.NSeries.CategoryData = "C1:C4"
'Guardar el archivo de Excel
workbook.Save("book1.xls")
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Series](../series)
* espacio de nombres [Aspose.Cells.Charts](../../aspose.cells.charts)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
