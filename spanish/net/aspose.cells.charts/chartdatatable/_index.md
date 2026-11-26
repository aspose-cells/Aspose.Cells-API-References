---
title: "Clase ChartDataTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.ChartDataTable. Representa una tabla de datos del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartdatatable/
---
## ChartDataTable class

Representa una tabla de datos del gráfico.

```csharp
public class ChartDataTable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/chartdatatable/autoscalefont/) { get; set; } | True si el texto en el objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor predeterminado es True. |
| [BackgroundMode](../../aspose.cells.charts/chartdatatable/backgroundmode/) { get; set; } | Obtiene y establece el modo de visualización del fondo |
| [Border](../../aspose.cells.charts/chartdatatable/border/) { get; } | Devuelve un objeto Border que representa el borde del objeto |
| [Font](../../aspose.cells.charts/chartdatatable/font/) { get; } | Obtiene un objeto [`Font`](./font/) que representa la configuración de fuente de la tabla de datos del gráfico especificada. |
| [HasBorderHorizontal](../../aspose.cells.charts/chartdatatable/hasborderhorizontal/) { get; set; } | (**Obsoleto.**) Verdadero si la tabla de datos del gráfico tiene bordes de celda horizontales |
| [HasBorderOutline](../../aspose.cells.charts/chartdatatable/hasborderoutline/) { get; set; } | (**Obsolete.**) Verdadero si la tabla de datos del gráfico tiene bordes de contorno |
| [HasBorderVertical](../../aspose.cells.charts/chartdatatable/hasbordervertical/) { get; set; } | (**Obsolete.**) Verdadero si la tabla de datos del gráfico tiene bordes verticales de celda |
| [HasHorizontalBorder](../../aspose.cells.charts/chartdatatable/hashorizontalborder/) { get; set; } | Verdadero si la tabla de datos del gráfico tiene bordes horizontales de celda |
| [HasOutlineBorder](../../aspose.cells.charts/chartdatatable/hasoutlineborder/) { get; set; } | Verdadero si la tabla de datos del gráfico tiene bordes de contorno |
| [HasVerticalBorder](../../aspose.cells.charts/chartdatatable/hasverticalborder/) { get; set; } | Verdadero si la tabla de datos del gráfico tiene bordes verticales de celda |
| [ShowLegendKey](../../aspose.cells.charts/chartdatatable/showlegendkey/) { get; set; } | Verdadero si la clave de la leyenda de la etiqueta de datos es visible. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDataTableDemo
    {
        public static void ChartDataTableExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Obteniendo la referencia de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar valores de muestra a celdas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);

            // Accediendo a la instancia del gráfico recién agregado
            Chart chart = worksheet.Charts[chartIndex];

            // Añadiendo NSeries (fuente de datos del gráfico) al gráfico desde la celda "A1" hasta "B3"
            chart.NSeries.Add("A1:B3", true);

            // Mostrando la tabla de datos
            chart.ShowDataTable = true;

            // Obteniendo la tabla de datos del gráfico
            ChartDataTable chartTable = chart.ChartDataTable;

            // Estableciendo propiedades de la tabla de datos del gráfico
            chartTable.Font.Color = Color.Red;
            chartTable.AutoScaleFont = true;
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.HasBorderOutline = true;
            chartTable.ShowLegendKey = false;

            // Guardando el archivo Excel
            workbook.Save("ChartDataTableExample.xlsx");
            workbook.Save("ChartDataTableExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


