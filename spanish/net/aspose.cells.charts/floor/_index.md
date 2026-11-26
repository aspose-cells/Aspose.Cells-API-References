---
title: "Clase Floor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.Floor. Encapsula el objeto que representa el piso de un gráfico 3D"
type: docs
url: /es/net/aspose.cells.charts/floor/
---
## Floor class

Encapsula el objeto que representa el piso de un gráfico 3D.

```csharp
public class Floor : Area
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Obtiene o establece el Color de fondo del [`Area`](../../aspose.cells.drawing/area/).(Heredado de [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Obtiene o establece el borde [`Line`](../../aspose.cells.drawing/line/). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Representa un objeto [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) que contiene propiedades de formato de relleno para el gráfico o forma especificados.(Heredado de [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Obtiene o establece el Color de primer plano.(Heredado de [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Representa el formato del área.(Heredado de [`Area`](../../aspose.cells.drawing/area/).) |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Si la propiedad es verdadera y el valor del punto del gráfico es un número negativo, el color de primer plano y el color de fondo se intercambiarán.(Heredado de [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro).(Heredado de [`Area`](../../aspose.cells.drawing/area/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FloorDemo
    {
        public static void FloorExample()
        {
            // Instanciar el objeto libro de trabajo
            Workbook workbook = new Workbook();

            // Obtener colección de celdas
            Cells cells = workbook.Worksheets[0].Cells;

            // Colocar valores en celdas
            cells["A1"].PutValue(1);
            cells["A2"].PutValue(2);
            cells["A3"].PutValue(3);

            // Obtener colección de gráficos
            ChartCollection charts = workbook.Worksheets[0].Charts;

            // Agregar un nuevo gráfico
            int index = charts.Add(ChartType.Column3DStacked, 5, 0, 15, 5);

            // Obtener el gráfico recién agregado
            Chart chart = charts[index];

            // Establecer nseries del gráfico
            chart.NSeries.Add("A1:A3", true);

            // Mostrar etiquetas de datos
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Obtener el piso del gráfico
            Floor floor = chart.Floor;

            // Establecer el borde del piso como rojo
            floor.Border.Color = Color.Red;

            // Establecer formato de relleno
            floor.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);

            // Establecer propiedades adicionales
            floor.BackgroundColor = Color.LightBlue;
            floor.ForegroundColor = Color.DarkBlue;
            floor.Formatting = FormattingType.Custom;
            floor.InvertIfNegative = true;
            floor.Transparency = 0.5;

            // Guardar el archivo
            workbook.Save(@"FloorExample.xlsx");
            workbook.Save(@"FloorExample.pdf");
        }
    }
}
```

### Ver también

* class [Area](../../aspose.cells.drawing/area/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


