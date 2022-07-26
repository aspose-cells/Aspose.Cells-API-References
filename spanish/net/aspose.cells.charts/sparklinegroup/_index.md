---
title: SparklineGroup
second_title: Referencia de API de Aspose.Cells para .NET
description: Sparkline./sparkline se organiza en grupo minigráfico. SparklineGroup contiene un número variable de minigráficos. Un grupo de minigráficos especifica el tipo la configuración de visualización y la configuración del eje para los minigráficos.
type: docs
weight: 880
url: /es/net/aspose.cells.charts/sparklinegroup/
---
## SparklineGroup class

[`Sparkline`](../sparkline) se organiza en grupo minigráfico. SparklineGroup contiene un número variable de minigráficos. Un grupo de minigráficos especifica el tipo, la configuración de visualización y la configuración del eje para los minigráficos.

```csharp
public class SparklineGroup
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DisplayHidden](../../aspose.cells.charts/sparklinegroup/displayhidden) { get; set; } | Indica si mostrar datos en filas y columnas ocultas. |
| [FirstPointColor](../../aspose.cells.charts/sparklinegroup/firstpointcolor) { get; set; } | Obtiene y establece el color del primer punto de datos en el grupo de minigráficos. |
| [HighPointColor](../../aspose.cells.charts/sparklinegroup/highpointcolor) { get; set; } | Obtiene y establece el color de los puntos más altos de datos en el grupo de minigráficos. |
| [HorizontalAxisColor](../../aspose.cells.charts/sparklinegroup/horizontalaxiscolor) { get; set; } | Obtiene y establece el color del eje horizontal en el grupo de minigráficos. |
| [HorizontalAxisDateRange](../../aspose.cells.charts/sparklinegroup/horizontalaxisdaterange) { get; set; } | Representa el rango que contiene los valores de fecha para los datos del minigráfico. |
| [LastPointColor](../../aspose.cells.charts/sparklinegroup/lastpointcolor) { get; set; } | Obtiene y establece el color del último punto de datos en el grupo minigráfico. |
| [LineWeight](../../aspose.cells.charts/sparklinegroup/lineweight) { get; set; } | Obtiene y establece el grosor de línea en cada minigráfico de línea en el grupo de minigráficos, en la unidad de puntos. |
| [LowPointColor](../../aspose.cells.charts/sparklinegroup/lowpointcolor) { get; set; } | Obtiene y establece el color de los puntos más bajos de datos en el grupo de minigráficos. |
| [MarkersColor](../../aspose.cells.charts/sparklinegroup/markerscolor) { get; set; } | Obtiene y establece el color de los puntos en cada minigráfico de línea en el grupo de minigráficos. |
| [NegativePointsColor](../../aspose.cells.charts/sparklinegroup/negativepointscolor) { get; set; } | Obtiene y establece el color de los valores negativos en el grupo de minigráficos. |
| [PlotEmptyCellsType](../../aspose.cells.charts/sparklinegroup/plotemptycellstype) { get; set; } | Indica cómo trazar celdas vacías. |
| [PlotRightToLeft](../../aspose.cells.charts/sparklinegroup/plotrighttoleft) { get; set; } | Indica si los datos del gráfico son de derecha a izquierda. |
| [PresetStyle](../../aspose.cells.charts/sparklinegroup/presetstyle) { get; set; } | Obtiene y establece el tipo de estilo preestablecido del grupo de minigráficos. |
| [SeriesColor](../../aspose.cells.charts/sparklinegroup/seriescolor) { get; set; } | Obtiene y establece el color de los minigráficos en el grupo de minigráficos. |
| [ShowFirstPoint](../../aspose.cells.charts/sparklinegroup/showfirstpoint) { get; set; } | Indica si resaltar el primer punto de datos en el grupo minigráfico. |
| [ShowHighPoint](../../aspose.cells.charts/sparklinegroup/showhighpoint) { get; set; } | Indica si resaltar los puntos más altos de datos en el grupo de minigráficos. |
| [ShowHorizontalAxis](../../aspose.cells.charts/sparklinegroup/showhorizontalaxis) { get; set; } | Indica si mostrar el eje horizontal del minigráfico. El eje horizontal aparece si el minigráfico tiene datos que cruzan el eje cero. |
| [ShowLastPoint](../../aspose.cells.charts/sparklinegroup/showlastpoint) { get; set; } | Indica si resaltar el último punto de datos en el grupo minigráfico. |
| [ShowLowPoint](../../aspose.cells.charts/sparklinegroup/showlowpoint) { get; set; } | Indica si resaltar los puntos más bajos de datos en el grupo de minigráficos. |
| [ShowMarkers](../../aspose.cells.charts/sparklinegroup/showmarkers) { get; set; } | Indica si resaltar cada punto en cada minigráfico de línea en el grupo de minigráficos. |
| [ShowNegativePoints](../../aspose.cells.charts/sparklinegroup/shownegativepoints) { get; set; } | Indica si resaltar los valores negativos en el grupo de minigráficos con un color o marcador diferente. |
| [SparklineCollection](../../aspose.cells.charts/sparklinegroup/sparklinecollection) { get; } | Obtiene el[`SparklineCollection`](./sparklinecollection) objeto del minigráfico group. |
| [Type](../../aspose.cells.charts/sparklinegroup/type) { get; set; } | Indica el tipo de minigráfico del grupo de minigráficos. |
| [VerticalAxisMaxValue](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvalue) { get; set; } | Obtiene y establece el valor máximo personalizado para el eje vertical. |
| [VerticalAxisMaxValueType](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvaluetype) { get; set; } | Representa el tipo de valor máximo del eje vertical. |
| [VerticalAxisMinValue](../../aspose.cells.charts/sparklinegroup/verticalaxisminvalue) { get; set; } | Obtiene y establece el valor mínimo personalizado para el eje vertical. |
| [VerticalAxisMinValueType](../../aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype) { get; set; } | Representa el tipo de valor mínimo del eje vertical. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ResetRanges](../../aspose.cells.charts/sparklinegroup/resetranges)(string, bool, CellArea) | Restablece el rango de datos y el rango de ubicación del grupo minigráfico. Este método borrará los elementos minigráficos originales del grupo y creará nuevos elementos minigráficos para los nuevos rangos. |

### Ejemplos

```csharp
[C#]
 Workbook book = new Workbook(); 
 Worksheet sheet = book.Worksheets[0];

 sheet.Cells["A1"].PutValue(5);
 sheet.Cells["B1"].PutValue(2);
 sheet.Cells["C1"].PutValue(1);
 sheet.Cells["D1"].PutValue(3);
 
 // Definir el área de celda
 CellArea ca = new CellArea();
 ca.StartColumn = 4;
 ca.EndColumn = 4;
 ca.StartRow = 0;
 ca.EndRow = 0;
 int idx = sheet.SparklineGroupCollection.Add(Aspose.Cells.Charts.SparklineType.Line, "A1:D1", false, ca);
 SparklineGroup group = sheet.SparklineGroupCollection[idx];
 group.SparklineCollection.Add(sheet.Name + "!A1:D1", 0, 4);
 // Crear color de celdas
 CellsColor clr = book.CreateCellsColor();
 clr.Color = Color.Orange;
 group.SeriesColor = clr;

 // establecer que los puntos altos sean de color verde y los puntos bajos de color rojo
 group.ShowHighPoint = true;
 group.ShowLowPoint = true;
 group.HighPointColor.Color = Color.Green;
 group.LowPointColor.Color = Color.Red;
 // establece el grosor de línea 
 group.LineWeight = 1.0;
 book.Save("output.xlsx", SaveFormat.Xlsx);
```

### Ver también

* espacio de nombres [Aspose.Cells.Charts](../../aspose.cells.charts)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
