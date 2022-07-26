---
title: ErrorBar
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa la barra de error de la serie de datos.
type: docs
weight: 630
url: /es/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Representa la barra de error de la serie de datos.

```csharp
public class ErrorBar : Line
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount) { get; set; } | Representa la cantidad de barra de error.  La cantidad debe ser mayor o igual a cero. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Especifica la longitud de la punta de flecha para el comienzo de una línea. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Especifica el ancho de la punta de flecha para el comienzo de una línea. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Especifica una punta de flecha para el comienzo de una línea. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Especifica las mayúsculas finales. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | Representa elColor de la linea. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Especifica el tipo de línea compuesta |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Especifica el tipo de línea discontinua |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype) { get; set; } | Representa el tipo de visualización de la barra de error. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Especifica la longitud de la punta de flecha al final de una línea. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Especifica el ancho de la punta de flecha para el final de una línea. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Especifica una punta de flecha para el final de una línea. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Obtiene o establece el tipo de formato. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Representa relleno degradado. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indica si este estilo de línea se asigna automáticamente. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indica si el color de la línea se asigna automáticamente. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Representa si la línea es visible. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Especifica las tapas de unión. |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue) { get; set; } | Representa la cantidad de error negativa cuando el tipo de barra de error es Personalizado. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue) { get; set; } | Representa una cantidad de error positiva cuando el tipo de barra de error es Personalizado. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop) { get; set; } | Indica si hay error de formato en barras con T-top. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Representa el estilo de la línea. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Obtiene y establece el color del tema. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Devuelve o establece el grado de transparencia de la línea como un valor de 0,0 (opaco) a 1,0 (transparente). |
| [Type](../../aspose.cells.charts/errorbar/type) { get; set; } | Representa el tipo de cantidad de la barra de error. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Obtiene o establece el[`WeightType`](../../aspose.cells.drawing/weighttype) de la linea. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Obtiene o establece el peso de la línea en unidades de puntos. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Obtiene o establece el grosor de la línea en unidades de píxeles. |

### Ejemplos

```csharp
[C#]
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["a1"].PutValue(2);
cells["a2"].PutValue(5);
cells["a3"].PutValue(3);
cells["a4"].PutValue(6);
cells["b1"].PutValue(4);
cells["b2"].PutValue(3);
cells["b3"].PutValue(6);
cells["b4"].PutValue(7);

cells["C1"].PutValue("Q1");
cells["C2"].PutValue("Q2");
cells["C3"].PutValue("Y1");
cells["C4"].PutValue("Y2");

int chartIndex = excel.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);

Chart chart = excel.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);

chart.NSeries.CategoryData = "C1:C4";

for(int i = 0; i < chart.NSeries.Count; i ++)
{
	ASeries aseries = chart.NSeries[i];
	aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
	aseries.YErrorBar.Type = ErrorBarType.FixedValue;
	aseries.YErrorBar.Amount = 5;
}

[Visual Basic]
Dim workbook As Workbook =  New Workbook() 
Dim cells As Cells =  workbook.Worksheets(0).Cells 
cells("a1").PutValue(2)
cells("a2").PutValue(5)
cells("a3").PutValue(3)
cells("a4").PutValue(6)
cells("b1").PutValue(4)
cells("b2").PutValue(3)
cells("b3").PutValue(6)
cells("b4").PutValue(7)

cells("C1").PutValue("Q1")
cells("C2").PutValue("Q2")
cells("C3").PutValue("Y1")
cells("C4").PutValue("Y2")

Dim chartIndex As Integer =  excel.Worksheets(0).Charts.Add(ChartType.Column,11,0,27,10) 

Dim chart As Chart =  excel.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:B4", True)

chart.NSeries.CategoryData = "C1:C4"

Dim i As Integer
For  i = 0 To chart.NSeries.Count - 1
Dim aseries As ASeries =  chart.NSeries(i) 
aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus
aseries.YErrorBar.Type = ErrorBarType.FixedValue
aseries.YErrorBar.Amount = 5
Next
```

### Ver también

* class [Line](../../aspose.cells.drawing/line)
* espacio de nombres [Aspose.Cells.Charts](../../aspose.cells.charts)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
