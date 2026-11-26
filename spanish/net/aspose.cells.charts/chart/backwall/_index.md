---
title: "Chart.BackWall"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Devuelve un objeto Walls que representa la pared trasera de un gráfico 3D"
type: docs
url: /es/net/aspose.cells.charts/chart/backwall/
---
## Chart.BackWall property

Devuelve un objeto [`Walls`](../walls/) que representa la pared trasera de un gráfico 3-D.

```csharp
public Walls BackWall { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyBackWallDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);

            // Agregar un gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Asegúrese de que sea un gráfico 3D
            if (chart.Is3D)
            {
                // Obtener el objeto BackWall
                Walls backWall = chart.BackWall;

                // Mostrar algunas propiedades del BackWall
                Console.WriteLine("BackWall properties:");
                Console.WriteLine("CenterX: " + backWall.CenterX);
                Console.WriteLine("CenterY: " + backWall.CenterY);
                Console.WriteLine("Width: " + backWall.Width);
                Console.WriteLine("Height: " + backWall.Height);

                // Formatear el BackWall
                backWall.FillFormat.SetOneColorGradient(
                    System.Drawing.Color.LightBlue, 
                    0.5, // Changed from GradientStyleType to double for degree parameter
                    Aspose.Cells.Drawing.GradientStyleType.Horizontal, 
                    1); // Changed from 0.5 to int for variant parameter

                // Establecer propiedades del borde
                backWall.Border.Color = System.Drawing.Color.DarkBlue;
                backWall.Border.Weight = Aspose.Cells.Drawing.WeightType.MediumLine;
            }

            // Guarda el libro de trabajo
            workbook.Save("ChartPropertyBackWallDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


