---
title: "Chart.RotationAngle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Representa la rotación de la vista del gráfico 3D, la rotación del área de trazado alrededor del eje Z en grados"
type: docs
url: /es/net/aspose.cells.charts/chart/rotationangle/
---
## Chart.RotationAngle property

Representa la rotación de la vista del gráfico 3-D (la rotación del área de trazado alrededor del eje z, en grados).

```csharp
public int RotationAngle { get; set; }
```

### Observaciones

El valor de esta propiedad debe estar entre 0 y 360, excepto para los gráficos de barras 3D, donde el valor debe estar entre 0 y 44. El valor predeterminado es 20. Se aplica solo a gráficos 3D.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRotationAngleDemo
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
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer el ángulo de rotación a 45 grados
            chart.RotationAngle = 45;

            // Guarda el libro de trabajo
            workbook.Save("ChartRotationAngleDemo.xlsx");

            Console.WriteLine("Chart with rotation angle created successfully.");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


