---
title: ChartDataTable
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa una tabla de datos de gráficos.
type: docs
weight: 460
url: /es/net/aspose.cells.charts/chartdatatable/
---
## ChartDataTable class

Representa una tabla de datos de gráficos.

```csharp
public class ChartDataTable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/chartdatatable/autoscalefont) { get; set; } | Verdadero si el texto del objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor predeterminado es Verdadero. |
| [BackgroundMode](../../aspose.cells.charts/chartdatatable/backgroundmode) { get; set; } | Obtiene y establece el modo de visualización del fondo |
| [Border](../../aspose.cells.charts/chartdatatable/border) { get; } | Devuelve un objeto Border que representa el borde del object |
| [Font](../../aspose.cells.charts/chartdatatable/font) { get; } | Obtiene un[`Font`](./font) objeto que representa la configuración de fuente de la tabla de datos del gráfico especificada. |
| [HasBorderHorizontal](../../aspose.cells.charts/chartdatatable/hasborderhorizontal) { get; set; } | Verdadero si la tabla de datos del gráfico tiene bordes de celda horizontales |
| [HasBorderOutline](../../aspose.cells.charts/chartdatatable/hasborderoutline) { get; set; } | Verdadero si la tabla de datos del gráfico tiene bordes de contorno |
| [HasBorderVertical](../../aspose.cells.charts/chartdatatable/hasbordervertical) { get; set; } | Verdadero si la tabla de datos del gráfico tiene bordes de celda verticales |
| [ShowLegendKey](../../aspose.cells.charts/chartdatatable/showlegendkey) { get; set; } | Verdadero si la clave de la leyenda de la etiqueta de datos está visible. |

### Ejemplos

```csharp

[C#]

// Instanciando un objeto Workbook
Workbook workbook = new Workbook();

//Obteniendo la referencia de la primera hoja de cálculo
Worksheet worksheet = workbook.Worksheets[0];

// Agregar un valor de muestra a la celda "A1"
worksheet.Cells["A1"].PutValue(50);

// Agregar un valor de muestra a la celda "A2"
worksheet.Cells["A2"].PutValue(100);

// Agregar un valor de muestra a la celda "A3"
worksheet.Cells["A3"].PutValue(150);

// Agregar un valor de muestra a la celda "B1"
worksheet.Cells["B1"].PutValue(60);

// Agregar un valor de muestra a la celda "B2"
worksheet.Cells["B2"].PutValue(32);

// Agregar un valor de muestra a la celda "B3"
worksheet.Cells["B3"].PutValue(50);

//Añadiendo un gráfico a la hoja de trabajo
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);

//Accediendo a la instancia del gráfico recién agregado
Chart chart = worksheet.Charts[chartIndex];

// Agregar NSeries (fuente de datos del gráfico) al gráfico que va desde la celda "A1" hasta la celda "B3"
chart.NSeries.Add("A1:B3", true);

chart.ShowDataTable = true;

//Obteniendo tabla de gráfico
ChartDataTable chartTable = chart.ChartDataTable;

//Configuración del color de la fuente de la tabla del gráfico
chartTable.Font.Color = System.Drawing.Color.Red;

//Configuración de las opciones de visibilidad de la clave de leyenda
chartTable.ShowLegendKey = false;

//Guardando el archivo de Excel
workbook.Save("book1.xls");

[VB.NET]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()

'Obtención de la referencia de la primera hoja de cálculo
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)

'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)

'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)

'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)

'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)

'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)

'Adición de un gráfico a la hoja de cálculo
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10)

'Acceso a la instancia del gráfico recién agregado
Dim chart As Chart = worksheet.Charts(chartIndex)

'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)

chart.ShowDataTable = True

'Obtener tabla de gráficos
Dim chartTable As ChartDataTable = chart.ChartDataTable

'Configuración del color de fuente de la tabla del gráfico
chartTable.Font.Color = System.Drawing.Color.Red

'Configuración de las opciones de visibilidad de la clave de leyenda
chartTable.ShowLegendKey = False

'Guardar el archivo de Excel
workbook.Save("book1.xls")

```

### Ver también

* espacio de nombres [Aspose.Cells.Charts](../../aspose.cells.charts)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
