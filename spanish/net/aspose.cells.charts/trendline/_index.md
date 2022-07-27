---
title: Trendline
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa una línea de tendencia en un gráfico.
type: docs
weight: 980
url: /es/net/aspose.cells.charts/trendline/
---
## Trendline class

Representa una línea de tendencia en un gráfico.

```csharp
public class Trendline : Line
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Backward](../../aspose.cells.charts/trendline/backward) { get; set; } | Devuelve o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia atrás. El número de periodos debe ser mayor o igual a cero. Si el tipo de gráfico es columna, el número de periodos debe estar entre 0 y 0,5 |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Especifica la longitud de la punta de flecha para el comienzo de una línea. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Especifica el ancho de la punta de flecha para el comienzo de una línea. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Especifica una punta de flecha para el comienzo de una línea. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Especifica las mayúsculas finales. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | Representa elColor de la linea. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Especifica el tipo de línea compuesta |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Especifica el tipo de línea discontinua |
| [DataLabels](../../aspose.cells.charts/trendline/datalabels) { get; } | Representa el objeto DataLabels para la serie especificada. |
| [DisplayEquation](../../aspose.cells.charts/trendline/displayequation) { get; set; } | Representa si la ecuación de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que el valor R-cuadrado). Establecer esta propiedad en True activa automáticamente las etiquetas de datos. |
| [DisplayRSquared](../../aspose.cells.charts/trendline/displayrsquared) { get; set; } | Representa si el valor R cuadrado de la línea de tendencia se muestra en el gráfico (en la misma etiqueta de datos que la ecuación). Establecer esta propiedad en True activa automáticamente las etiquetas de datos. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Especifica la longitud de la punta de flecha al final de una línea. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Especifica el ancho de la punta de flecha para el final de una línea. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Especifica una punta de flecha para el final de una línea. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Obtiene o establece el tipo de formato. |
| [Forward](../../aspose.cells.charts/trendline/forward) { get; set; } | Devuelve o establece el número de períodos (o unidades en un gráfico de dispersión) que la línea de tendencia se extiende hacia adelante. El número de períodos debe ser mayor o igual a cero. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Representa relleno degradado. |
| [Intercept](../../aspose.cells.charts/trendline/intercept) { get; set; } | Devuelve o establece el punto donde la línea de tendencia cruza el eje de valores. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indica si este estilo de línea se asigna automáticamente. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indica si el color de la línea se asigna automáticamente. |
| [IsNameAuto](../../aspose.cells.charts/trendline/isnameauto) { get; set; } | Devuelve si Microsoft Excel determina automáticamente el nombre de la línea de tendencia. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Representa si la línea es visible. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Especifica las tapas de unión. |
| [LegendEntry](../../aspose.cells.charts/trendline/legendentry) { get; } | Obtiene la entrada de la leyenda de acuerdo con esta línea de tendencia |
| [Name](../../aspose.cells.charts/trendline/name) { get; set; } | Devuelve el nombre de la línea de tendencia. |
| [Order](../../aspose.cells.charts/trendline/order) { get; set; } | Devuelve o establece el orden de la línea de tendencia (un número entero mayor que 1) cuando el tipo de línea de tendencia es Polinomial. El pedido debe estar entre 2 y 6. |
| [Period](../../aspose.cells.charts/trendline/period) { get; set; } | Devuelve o establece el período para la línea de tendencia de la media móvil. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Representa el estilo de la línea. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Obtiene y establece el color del tema. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Devuelve o establece el grado de transparencia de la línea como un valor de 0,0 (opaco) a 1,0 (transparente). |
| [Type](../../aspose.cells.charts/trendline/type) { get; } | Devuelve el tipo de línea de tendencia. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Obtiene o establece el[`WeightType`](../../aspose.cells.drawing/weighttype) de la linea. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Obtiene o establece el peso de la línea en unidades de puntos. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Obtiene o establece el grosor de la línea en unidades de píxeles. |

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
//añadiendo una línea de tendencia lineal
int index = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[index];
//Establecer el nombre personalizado de la línea de tendencia.
trendline.Name = "Linear";
//Mostrando la ecuación en el gráfico
trendline.DisplayEquation = true;
//Mostrando el valor R-Squared en el gráfico
trendline.DisplayRSquared = true;
//Guardando el archivo de Excel
workbook.Save("book1.xls");

[Visual Basic]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()
'Agregar una nueva hoja de cálculo al objeto de Excel
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
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
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Acceso a la instancia del gráfico recién agregado
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'Configuración de la fuente de datos para los datos de categoría de NSeries
Chart.NSeries.CategoryData = "C1:C4"
'agregar una línea de tendencia lineal
Dim index As Int32 = chart.NSeries(0).TrendLines.Add(TrendlineType.Linear)
Dim trendline As Trendline = chart.NSeries(0).TrendLines(index)
'Configuración del nombre personalizado de la línea de tendencia.
trendline.Name = "Linear"
'Visualización de la ecuación en el gráfico
trendline.DisplayEquation = True
'Visualización del valor R-Squared en el gráfico
trendline.DisplayRSquared = True
'Guardar el archivo de Excel
workbook.Save("book1.xls")
```

### Ver también

* class [Line](../../aspose.cells.drawing/line)
* espacio de nombres [Aspose.Cells.Charts](../../aspose.cells.charts)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
