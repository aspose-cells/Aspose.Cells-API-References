---
title: "Chart.RightAngleAxes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Verdadero si los ejes del gráfico están a ángulos rectos. Se aplica solo a gráficos 3D, excepto Column3D y gráficos de pastel 3D"
type: docs
url: /es/net/aspose.cells.charts/chart/rightangleaxes/
---
## Chart.RightAngleAxes property

True si los ejes del gráfico forman ángulos rectos. Se aplica solo a gráficos 3-D (excepto Column3D y gráficos de pastel 3-D).

```csharp
public bool RightAngleAxes { get; set; }
```

### Observaciones

Si esta propiedad es Verdadera, se ignora la propiedad Perspective.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRightAngleAxesDemo
    {
        public static void Run()
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
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Agregar un gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demostrar la propiedad RightAngleAxes
            chart.RightAngleAxes = true;
            Console.WriteLine("RightAngleAxes is set to: " + chart.RightAngleAxes);

            // Guarda el libro de trabajo
            workbook.Save("RightAngleAxesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


