---
title: Title
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula el objeto que representa el título del gráfico o eje.
type: docs
weight: 970
url: /es/net/aspose.cells.charts/title/
---
## Title class

Encapsula el objeto que representa el título del gráfico o eje.

```csharp
public class Title : ChartTextFrame
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Obtiene el[`área`](../chartframe/area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | Verdadero si el texto del objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor por defecto es verdadero. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Obtiene y establece el modo de visualización del fondo |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Obtiene el[`borde`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Representa la altura de la posición predeterminada |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Representa el ancho de la posición predeterminada |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Representa x de la posición predeterminada |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Representa y de la posición predeterminada |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Obtiene y establece la dirección del texto. |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | Obtiene un[`Font`](../chartframe/font) objeto del objeto ChartFrame especificado. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Obtiene o establece la altura del marco en unidades de 1/4000 del área del gráfico. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indica si el marco del gráfico tiene un tamaño automático. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Indica que el texto se genera automáticamente. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indica si la posición predeterminada (DefaultX, DefaultY, DefaultWidth y DefaultHeight) está configurada. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Indica si se eliminan estas etiquetas de datos. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indica si el tamaño del área de trazado incluye las marcas y las etiquetas de los ejes. Falso especifica que el tamaño determinará el tamaño del área de trazado, las marcas y las etiquetas de los ejes. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Obtiene o establece si una forma debe ajustarse automáticamente para contener completamente el texto descrito en ella. El ajuste automático es cuando el texto dentro de una forma se escala para contener todo el texto dentro. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Obtiene o establece un valor que indica si el texto está ajustado. |
| [IsVisible](../../aspose.cells.charts/title/isvisible) { get; set; } | Representa si el título es visible. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Obtiene y establece una referencia a la hoja de cálculo. |
| [OverLay](../../aspose.cells.charts/title/overlay) { get; set; } | Representa el título centrado superpuesto en el gráfico sin cambiar el tamaño del gráfico. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Representa el orden de lectura del texto. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Representa el ángulo de rotación del texto. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Verdadero si el marco tiene sombra. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Obtiene el[`ShapeProperties`](../chartframe/shapeproperties) objeto. |
| override [Text](../../aspose.cells.charts/title/text) { get; set; } | Obtiene o establece el texto de la etiqueta de la unidad de visualización. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Obtiene y establece la alineación horizontal del texto. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Obtiene o establece la alineación vertical del texto de text. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Obtiene o establece el ancho del marco en unidades de 1/4000 del área del gráfico. |
| override [X](../../aspose.cells.charts/title/x) { get; set; } | Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| override [Y](../../aspose.cells.charts/title/y) { get; set; } | Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Characters](../../aspose.cells.charts/title/characters#characters_1)() | Obtiene el formato de texto enriquecido de este Título. |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Establece la posición del marco en automático |

### Ejemplos

```csharp

[C#]

Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];

//Establecer el título de un gráfico
chart.Title.Text = "Title";
//Establecer el color de fuente del título del gráfico en azul
chart.Title.Font.Color = Color.Blue;
//Establecer el título del eje de categoría del gráfico
chart.CategoryAxis.Title.Text = "Category";
//Establecer el título del eje de valores del gráfico
chart.ValueAxis.Title.Text = "Value";

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)    ///
Dim chart as Chart = sheet.Charts(chartIndex)

'Establecer el título de un gráfico
chart.Title.Text = "Title"
'Establecer el color de fuente del título del gráfico en azul
chart.Title.Font.Color = Color.Blue
'Establecer el título del eje de categoría del gráfico
chart.CategoryAxis.Title.Text = "Category"
'Establecer el título del eje de valor del gráfico
chart.ValueAxis.Title.Text = "Value"

```

### Ver también

* class [ChartTextFrame](../charttextframe)
* espacio de nombres [Aspose.Cells.Charts](../../aspose.cells.charts)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
