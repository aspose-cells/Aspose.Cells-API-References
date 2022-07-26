---
title: Line
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula el objeto que representa el formato de línea.
type: docs
weight: 2200
url: /es/net/aspose.cells.drawing/line/
---
## Line class

Encapsula el objeto que representa el formato de línea.

```csharp
public class Line
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Especifica la longitud de la punta de flecha para el comienzo de una línea. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Especifica el ancho de la punta de flecha para el comienzo de una línea. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Especifica una punta de flecha para el comienzo de una línea. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Especifica las mayúsculas finales. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | Representa elColor de la linea. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Especifica el tipo de línea compuesta |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Especifica el tipo de línea discontinua |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Especifica la longitud de la punta de flecha al final de una línea. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Especifica el ancho de la punta de flecha para el final de una línea. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Especifica una punta de flecha para el final de una línea. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Obtiene o establece el tipo de formato. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Representa relleno degradado. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indica si este estilo de línea se asigna automáticamente. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indica si el color de la línea se asigna automáticamente. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Representa si la línea es visible. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Especifica las tapas de unión. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Representa el estilo de la línea. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Obtiene y establece el color del tema. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Devuelve o establece el grado de transparencia de la línea como un valor de 0,0 (opaco) a 1,0 (transparente). |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Obtiene o establece el[`WeightType`](../weighttype) de la linea. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Obtiene o establece el peso de la línea en unidades de puntos. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Obtiene o establece el grosor de la línea en unidades de píxeles. |

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

int chartIndex = sheet.Charts.Add(ChartType.Line, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];
//Aplicando un estilo de línea punteada en las líneas de una NSeries
chart.NSeries[0].Border.Style = LineType.Dot;
chart.NSeries[0].Border.Color = Color.Red;
//Aplicando un estilo de marcador triangular en los marcadores de datos de una NSeries
chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Triangle;
//Estableciendo el peso de todas las líneas en un NSeries a medio
chart.NSeries[0].Border.Weight = WeightType.MediumLine;

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
'Aplicar un estilo de línea de puntos en las líneas de un NSeries
chart.NSeries(0).Border.Style = LineType.Dot
chart.NSeries(0).Border.Color = Color.Red
'Aplicar un estilo de marcador triangular en los marcadores de datos de un NSeries
chart.NSeries(0).Marker.MarkerStyle = ChartMarkerType.Triangle
'Establecer el peso de todas las líneas en un NSeries a medio
chart.NSeries(0).Border.Weight = WeightType.MediumLine
```

### Ver también

* espacio de nombres [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
