---
title: Legend
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula el objeto que representa la leyenda del gráfico.
type: docs
weight: 690
url: /es/net/aspose.cells.charts/legend/
---
## Legend class

Encapsula el objeto que representa la leyenda del gráfico.

```csharp
public class Legend : ChartTextFrame
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
| [IsOverLay](../../aspose.cells.charts/legend/isoverlay) { get; set; } | Obtiene o establece si se permitirá que otros elementos del gráfico se superpongan a este elemento del gráfico. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Obtiene o establece si una forma debe ajustarse automáticamente para contener completamente el texto descrito en ella. El ajuste automático es cuando el texto dentro de una forma se escala para contener todo el texto dentro. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Obtiene o establece un valor que indica si el texto está ajustado. |
| [LegendEntries](../../aspose.cells.charts/legend/legendentries) { get; } | Obtiene una colección de todos los objetos LegendEntry en la leyenda del gráfico especificado. No se admite la configuración de las entradas de leyenda del gráfico de superficie. Por lo tanto, devolverá un valor nulo si el tipo de gráfico es el tipo de gráfico de superficie. |
| [LegendEntriesLabels](../../aspose.cells.charts/legend/legendentrieslabels) { get; } | Obtiene las etiquetas de las entradas de la leyenda después de llamar al método Chart.Calculate(). |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Obtiene y establece una referencia a la hoja de cálculo. |
| [Position](../../aspose.cells.charts/legend/position) { get; set; } | Obtiene o establece el tipo de posición de la leyenda. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Representa el orden de lectura del texto. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Representa el ángulo de rotación del texto. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Verdadero si el marco tiene sombra. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Obtiene el[`ShapeProperties`](../chartframe/shapeproperties) objeto. |
| virtual [Text](../../aspose.cells.charts/charttextframe/text) { get; set; } | Obtiene o establece el texto del título de un marco. |
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
chart.SetChartDataRange("A1:B4", true);
//Establecemos el ancho y alto de la Leyenda
Legend legend = chart.Legend;

//La leyenda está en el lado derecho del gráfico de forma predeterminada.
//Si la leyenda está en el lado izquierdo o derecho del gráfico, la configuración de la propiedad Legend.X no tendrá efecto.
//Si la leyenda está en la parte superior o inferior del gráfico, la configuración de la propiedad Legend.Y no tendrá efecto.
legend.Y = 1500;
legend.Width = 50;
legend.Height = 50; 
//Establecer la posición de la leyenda
legend.Position = LegendPositionType.Left;

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
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex)
chart.SetChartDataRange("A1:B4", True);
 
'Set Legend's width and height
Dim legend as Legend = chart.Legend

'La leyenda está en el lado derecho del gráfico de forma predeterminada.
'Si la leyenda está en el lado izquierdo o derecho del gráfico, la configuración de la propiedad Legend.X no tendrá efecto.
'Si la leyenda está en la parte superior o inferior del gráfico, la configuración de la propiedad Legend.Y no tendrá efecto.
legend.Y = 1500
legend.Width = 50
legend.Height = 50
'Set legend's position
legend.Position = LegendPositionType.Left
```

### Ver también

* class [ChartTextFrame](../charttextframe)
* espacio de nombres [Aspose.Cells.Charts](../../aspose.cells.charts)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
