---
title: "Clase Walls"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.Walls. Encapsula el objeto que representa las paredes de un gráfico 3D"
type: docs
url: /es/net/aspose.cells.charts/walls/
---
## Walls class

Encapsula el objeto que representa las paredes de un gráfico 3D.

```csharp
public class Walls : Floor
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Obtiene o establece el Color de fondo del [`Area`](../../aspose.cells.drawing/area/).(Heredado de [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Obtiene o establece el borde [`Line`](../../aspose.cells.drawing/line/).(Heredado de [`Floor`](../floor/).) |
| [CenterX](../../aspose.cells.charts/walls/centerx/) { get; } | Obtiene la coordenada x de la esquina inferior izquierda del centro de la pared en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate(). |
| [CenterXPx](../../aspose.cells.charts/walls/centerxpx/) { get; } | Obtiene la coordenada x de la esquina inferior izquierda del centro de la pared en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [CenterY](../../aspose.cells.charts/walls/centery/) { get; } | Obtiene la coordenada y de la esquina inferior izquierda del centro de la pared en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate(). |
| [CenterYPx](../../aspose.cells.charts/walls/centerypx/) { get; } | Obtiene la coordenada y de la esquina inferior izquierda del centro de la pared en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [Depth](../../aspose.cells.charts/walls/depth/) { get; } | Obtiene la profundidad de adelante hacia atrás en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate(). |
| [DepthPx](../../aspose.cells.charts/walls/depthpx/) { get; } | Obtiene la profundidad de adelante a atrás en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Representa un objeto [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) que contiene propiedades de formato de relleno para el gráfico o forma especificados.(Heredado de [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Obtiene o establece el Color de primer plano.(Heredado de [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Representa el formato del área.(Heredado de [`Area`](../../aspose.cells.drawing/area/).) |
| [Height](../../aspose.cells.charts/walls/height/) { get; } | Obtiene la altura de arriba a abajo en unidades de 1/4000 de la altura del gráfico después de llamar al método Chart.Calculate(). |
| [HeightPx](../../aspose.cells.charts/walls/heightpx/) { get; } | Obtiene la altura de arriba a abajo en unidades de píxeles después de llamar al método Chart.Calculate(). |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Si la propiedad es verdadera y el valor del punto del gráfico es un número negativo, el color de primer plano y el color de fondo se intercambiarán.(Heredado de [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro).(Heredado de [`Area`](../../aspose.cells.drawing/area/).) |
| [Width](../../aspose.cells.charts/walls/width/) { get; } | Obtiene el ancho de izquierda a derecha en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate(). |
| [WidthPx](../../aspose.cells.charts/walls/widthpx/) { get; } | Obtiene el ancho de izquierda a derecha en unidades de píxeles después de llamar al método Chart.Calculate(). |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetCubePointCount](../../aspose.cells.charts/walls/getcubepointcount/)() | Obtiene el número de puntos del cubo después de llamar al método Chart.Calculate(). |
| [GetCubePointXPx](../../aspose.cells.charts/walls/getcubepointxpx/)(int) | Obtiene la coordenada x del punto ápex del cubo de paredes después de llamar al método Chart.Calculate(). El número de puntos ápex del cubo de paredes es ocho. |
| [GetCubePointYPx](../../aspose.cells.charts/walls/getcubepointypx/)(int) | Obtiene la coordenada y del punto ápex del cubo de paredes después de llamar al método Chart.Calculate(). El número de puntos ápex del cubo de paredes es ocho. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class WallsDemo
    {
        public static void WallsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico 3D a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para actualizar sus propiedades
            chart.Calculate();

            // Acceder a las paredes del gráfico 3D
            Walls walls = chart.Walls;

            // Establecer propiedades de las paredes
            walls.BackgroundColor = Color.LightBlue;
            walls.ForegroundColor = Color.DarkBlue;
            walls.Formatting = FormattingType.Custom;
            walls.InvertIfNegative = true;
            walls.Transparency = 0.5;

            // Acceder al borde de las paredes y establecer sus propiedades
            Line border = walls.Border;
            border.Color = Color.Red;
            border.Style = LineType.Solid;

            // Imprimir algunas propiedades de las paredes
            Console.WriteLine("CenterX: " + walls.CenterX);
            Console.WriteLine("CenterY: " + walls.CenterY);
            Console.WriteLine("Width: " + walls.Width);
            Console.WriteLine("Depth: " + walls.Depth);
            Console.WriteLine("Height: " + walls.Height);
            Console.WriteLine("CenterXPx: " + walls.CenterXPx);
            Console.WriteLine("CenterYPx: " + walls.CenterYPx);
            Console.WriteLine("WidthPx: " + walls.WidthPx);
            Console.WriteLine("DepthPx: " + walls.DepthPx);
            Console.WriteLine("HeightPx: " + walls.HeightPx);

            // Guarda el libro de trabajo
            workbook.Save("WallsExample.xlsx");
        }
    }
}
```

### Ver también

* class [Floor](../floor/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


