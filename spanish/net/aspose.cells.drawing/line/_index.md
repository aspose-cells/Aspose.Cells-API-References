---
title: "Clase Line"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Line. Encapsula el objeto que representa el formato de línea"
type: docs
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
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Especifica la longitud de la punta de flecha para el inicio de una línea. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Especifica el ancho de la punta de flecha para el inicio de una línea. |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Especifica una punta de flecha para el inicio de una línea. |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Especifica los extremos finales. |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Representa el color de la línea. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Especifica el tipo de línea compuesta |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Especifica el tipo de línea de guiones |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Especifica la longitud de la punta de flecha para el final de una línea. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Especifica el ancho de la punta de flecha para el final de una línea. |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Especifica una punta de flecha para el final de una línea. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Obtiene o establece el tipo de formato. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Representa el relleno degradado. |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Indica si este estilo de línea se asigna automáticamente. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Indica si el color de la línea se asigna automáticamente. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Representa si la línea es visible. |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Especifica las terminaciones de unión. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Representa el estilo de la línea. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Obtiene y establece el color del tema. |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Devuelve o establece el grado de transparencia de la línea como un valor de 0.0 (opaco) a 1.0 (claro). |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Obtiene o establece el [`WeightType`](../weighttype/) de la línea. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Obtiene o establece el grosor de la línea en unidades de puntos. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Obtiene o establece el peso de la línea en unidades de píxeles. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassLineDemo
    {
        public static void Run()
        {
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
            
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 9, 9, 21, 15);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            chart.NSeries.Add("B1:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            chart.NSeries[0].Border.Style = LineType.Dot;
            chart.NSeries[0].Border.Color = Color.Red;
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Triangle;
            chart.NSeries[0].Border.Weight = WeightType.MediumLine;
            
            workbook.Save("LineChartDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


