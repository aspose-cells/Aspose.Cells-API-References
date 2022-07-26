---
title: DisplayUnitLabel
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa la etiqueta de la unidad de visualización.
type: docs
weight: 600
url: /es/net/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class

Representa la etiqueta de la unidad de visualización.

```csharp
public class DisplayUnitLabel : ChartTextFrame
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Obtiene el[`área`](../chartframe/area) . |
| override [AutoScaleFont](../../aspose.cells.charts/displayunitlabel/autoscalefont) { get; set; } | Verdadero si el texto del objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor por defecto es verdadero. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Obtiene y establece el modo de visualización del fondo |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Obtiene el[`borde`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Representa la altura de la posición predeterminada |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Representa el ancho de la posición predeterminada |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Representa x de la posición predeterminada |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Representa y de la posición predeterminada |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Obtiene y establece la dirección del texto. |
| override [Font](../../aspose.cells.charts/displayunitlabel/font) { get; } | Obtiene un[`Font`](./font) objeto del objeto ChartFrame especificado. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Obtiene o establece la altura del marco en unidades de 1/4000 del área del gráfico. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indica si el marco del gráfico tiene un tamaño automático. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Indica que el texto se genera automáticamente. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indica si la posición predeterminada (DefaultX, DefaultY, DefaultWidth y DefaultHeight) está configurada. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Indica si se eliminan estas etiquetas de datos. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indica si el tamaño del área de trazado incluye las marcas y las etiquetas de los ejes. Falso especifica que el tamaño determinará el tamaño del área de trazado, las marcas y las etiquetas de los ejes. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Obtiene o establece si una forma debe ajustarse automáticamente para contener completamente el texto descrito en ella. El ajuste automático es cuando el texto dentro de una forma se escala para contener todo el texto dentro. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Obtiene o establece un valor que indica si el texto está ajustado. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Obtiene y establece una referencia a la hoja de cálculo. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Representa el orden de lectura del texto. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Representa el ángulo de rotación del texto. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Verdadero si el marco tiene sombra. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Obtiene el[`ShapeProperties`](../chartframe/shapeproperties) objeto. |
| override [Text](../../aspose.cells.charts/displayunitlabel/text) { get; set; } | Obtiene o establece el texto de la etiqueta de la unidad de visualización. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Obtiene y establece la alineación horizontal del texto. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Obtiene o establece la alineación vertical del texto de text. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Obtiene o establece el ancho del marco en unidades de 1/4000 del área del gráfico. |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Establece la posición del marco en automático |

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
//Configuración de la unidad de visualización del eje de valor (Y).
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;
//Configuración de la etiqueta de la unidad de visualización personalizada
displayUnitLabel.Text = "100";
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
'Configuración de la unidad de visualización del eje de valor (Y).
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds
Dim displayUnitLabel As DisplayUnitLabel = chart.ValueAxis.DisplayUnitLabel
'Configuración de la etiqueta de la unidad de visualización personalizada
displayUnitLabel.Text = "100"
'Guardar el archivo de Excel
workbook.Save("book1.xls")
```

### Ver también

* class [ChartTextFrame](../charttextframe)
* espacio de nombres [Aspose.Cells.Charts](../../aspose.cells.charts)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
