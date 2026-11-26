---
title: "Clase SparklineGroup"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.SparklineGroup. Sparkline está organizado en un grupo de sparkline. Un SparklineGroup contiene un número variable de elementos de sparkline. Un grupo de sparkline especifica la configuración de visualización del tipo y la configuración del eje para los sparklines"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/
---
## SparklineGroup class

[`Sparkline`](../sparkline/) is organized into a sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

```csharp
public class SparklineGroup
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DisplayHidden](../../aspose.cells.charts/sparklinegroup/displayhidden/) { get; set; } | Indica si se deben mostrar datos en filas y columnas ocultas. |
| [FirstPointColor](../../aspose.cells.charts/sparklinegroup/firstpointcolor/) { get; set; } | Obtiene y establece el color del primer punto de datos en el grupo de sparkline. |
| [HighPointColor](../../aspose.cells.charts/sparklinegroup/highpointcolor/) { get; set; } | Obtiene y establece el color de los puntos más altos de datos en el grupo de sparkline. |
| [HorizontalAxisColor](../../aspose.cells.charts/sparklinegroup/horizontalaxiscolor/) { get; set; } | Obtiene y establece el color del eje horizontal en el grupo de sparkline. |
| [HorizontalAxisDateRange](../../aspose.cells.charts/sparklinegroup/horizontalaxisdaterange/) { get; set; } | Representa el rango que contiene los valores de fecha para los datos de sparkline. |
| [LastPointColor](../../aspose.cells.charts/sparklinegroup/lastpointcolor/) { get; set; } | Obtiene y establece el color del último punto de datos en el grupo de sparkline. |
| [LineWeight](../../aspose.cells.charts/sparklinegroup/lineweight/) { get; set; } | Obtiene y establece el grosor de línea en cada sparkline de línea del grupo de sparkline, en unidades de puntos. |
| [LowPointColor](../../aspose.cells.charts/sparklinegroup/lowpointcolor/) { get; set; } | Obtiene y establece el color de los puntos más bajos de datos en el grupo de sparkline. |
| [MarkersColor](../../aspose.cells.charts/sparklinegroup/markerscolor/) { get; set; } | Obtiene y establece el color de los puntos en cada sparkline de línea del grupo de sparkline. |
| [NegativePointsColor](../../aspose.cells.charts/sparklinegroup/negativepointscolor/) { get; set; } | Obtiene y establece el color de los valores negativos en el grupo de sparkline. |
| [PlotEmptyCellsType](../../aspose.cells.charts/sparklinegroup/plotemptycellstype/) { get; set; } | Indica cómo trazar celdas vacías. |
| [PlotRightToLeft](../../aspose.cells.charts/sparklinegroup/plotrighttoleft/) { get; set; } | Indica si los datos del gráfico se presentan de derecha a izquierda. |
| [PresetStyle](../../aspose.cells.charts/sparklinegroup/presetstyle/) { get; set; } | Obtiene y establece el tipo de estilo predefinido del grupo de sparkline. |
| [SeriesColor](../../aspose.cells.charts/sparklinegroup/seriescolor/) { get; set; } | Obtiene y establece el color de los sparklines en el grupo de sparkline. |
| [ShowFirstPoint](../../aspose.cells.charts/sparklinegroup/showfirstpoint/) { get; set; } | Indica si se debe resaltar el primer punto de datos en el grupo de sparkline. |
| [ShowHighPoint](../../aspose.cells.charts/sparklinegroup/showhighpoint/) { get; set; } | Indica si se debe resaltar los puntos más altos de datos en el grupo de sparkline. |
| [ShowHorizontalAxis](../../aspose.cells.charts/sparklinegroup/showhorizontalaxis/) { get; set; } | Indica si se debe mostrar el eje horizontal del sparkline. El eje horizontal aparece si el sparkline tiene datos que cruzan el eje cero. |
| [ShowLastPoint](../../aspose.cells.charts/sparklinegroup/showlastpoint/) { get; set; } | Indica si se debe resaltar el último punto de datos en el grupo de sparkline. |
| [ShowLowPoint](../../aspose.cells.charts/sparklinegroup/showlowpoint/) { get; set; } | Indica si se debe resaltar los puntos más bajos de datos en el grupo de sparkline. |
| [ShowMarkers](../../aspose.cells.charts/sparklinegroup/showmarkers/) { get; set; } | Indica si se debe resaltar cada punto en cada línea sparkline en el grupo de sparkline. |
| [ShowNegativePoints](../../aspose.cells.charts/sparklinegroup/shownegativepoints/) { get; set; } | Indica si se deben resaltar los valores negativos en el grupo de sparkline con un color o marcador diferente. |
| [SparklineCollection](../../aspose.cells.charts/sparklinegroup/sparklinecollection/) { get; } | (**Obsolete.**) Obtiene la colección del objeto [`Sparkline`](../sparkline/). |
| [Sparklines](../../aspose.cells.charts/sparklinegroup/sparklines/) { get; } | Obtiene la colección del objeto [`Sparkline`](../sparkline/). |
| [Type](../../aspose.cells.charts/sparklinegroup/type/) { get; set; } | Indica el tipo de sparkline del grupo de sparkline. |
| [VerticalAxisMaxValue](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvalue/) { get; set; } | Obtiene y establece el valor máximo personalizado para el eje vertical. |
| [VerticalAxisMaxValueType](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvaluetype/) { get; set; } | Representa el tipo de valor máximo del eje vertical. |
| [VerticalAxisMinValue](../../aspose.cells.charts/sparklinegroup/verticalaxisminvalue/) { get; set; } | Obtiene y establece el valor mínimo personalizado para el eje vertical. |
| [VerticalAxisMinValueType](../../aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype/) { get; set; } | Representa el tipo de valor mínimo del eje vertical. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ResetRanges](../../aspose.cells.charts/sparklinegroup/resetranges/)(string, bool, CellArea) | Restablece el rango de datos y el rango de ubicación del grupo de sparkline. Este método borrará los elementos sparkline originales en el grupo y creará nuevos elementos sparkline para los nuevos rangos. |
| [SetVerticalAxisMaxValue](../../aspose.cells.charts/sparklinegroup/setverticalaxismaxvalue/)(SparklineAxisMinMaxType, double) | Establece el valor máximo personalizado para el eje vertical del sparkline con el tipo de valor de eje especificado. |
| [SetVerticalAxisMinValue](../../aspose.cells.charts/sparklinegroup/setverticalaxisminvalue/)(SparklineAxisMinMaxType, double) | Establece el valor mínimo personalizado para el eje vertical del sparkline con el tipo de valor de eje especificado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineGroupDemo
    {
        public static void SparklineGroupExample()
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
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Crea CellsColor para el color de la serie
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            // Establece que los puntos altos se coloreen de verde y los puntos bajos de rojo
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = Color.Green;
            group.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = Color.Red;
            group.LowPointColor = lowPointColor;

            // Establece el grosor de la línea
            group.LineWeight = 1.0;

            // Establecer propiedades adicionales
            group.PresetStyle = SparklinePresetStyleType.Style1;
            group.Type = SparklineType.Line;
            group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;
            group.DisplayHidden = true;
            group.ShowNegativePoints = true;
            CellsColor negativePointsColor = workbook.CreateCellsColor();
            negativePointsColor.Color = Color.Blue;
            group.NegativePointsColor = negativePointsColor;

            group.ShowFirstPoint = true;
            CellsColor firstPointColor = workbook.CreateCellsColor();
            firstPointColor.Color = Color.Purple;
            group.FirstPointColor = firstPointColor;

            group.ShowLastPoint = true;
            CellsColor lastPointColor = workbook.CreateCellsColor();
            lastPointColor.Color = Color.Yellow;
            group.LastPointColor = lastPointColor;

            group.ShowMarkers = true;
            CellsColor markersColor = workbook.CreateCellsColor();
            markersColor.Color = Color.Black;
            group.MarkersColor = markersColor;

            group.PlotRightToLeft = false;
            CellsColor horizontalAxisColor = workbook.CreateCellsColor();
            horizontalAxisColor.Color = Color.Gray;
            group.HorizontalAxisColor = horizontalAxisColor;

            group.ShowHorizontalAxis = true;
            group.HorizontalAxisDateRange = "A1:D1";
            group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            group.VerticalAxisMaxValue = 10.0;
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Group;
            group.VerticalAxisMinValue = 0.0;

            // Guarda el libro de trabajo
            workbook.Save("SparklineGroupExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


