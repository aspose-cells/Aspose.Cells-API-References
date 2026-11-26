---
title: "Chart.SideWall"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Devuelve un objeto Walls que representa la pared lateral de un gráfico 3D"
type: docs
url: /es/net/aspose.cells.charts/chart/sidewall/
---
## Chart.SideWall property

Devuelve un objeto [`Walls`](../walls/) que representa la pared lateral de un gráfico 3D.

```csharp
public Walls SideWall { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertySideWallDemo
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
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Agregar un gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.SetChartDataRange("A1:C4", true);

            // Acceder a la propiedad SideWall
            Walls sideWall = chart.SideWall;
            
            // Mostrar algunas propiedades del SideWall
            Console.WriteLine("SideWall properties:");
            Console.WriteLine("Width: " + sideWall.Width);
            Console.WriteLine("Height: " + sideWall.Height);
            Console.WriteLine("Depth: " + sideWall.Depth);

            // Calcular el gráfico para actualizar las dimensiones de la pared
            chart.Calculate();

            // Mostrar propiedades actualizadas después del cálculo
            Console.WriteLine("\nAfter Calculate():");
            Console.WriteLine("SideWall CenterX: " + sideWall.CenterX);
            Console.WriteLine("SideWall CenterY: " + sideWall.CenterY);
            Console.WriteLine("SideWall WidthPx: " + sideWall.WidthPx);
            Console.WriteLine("SideWall HeightPx: " + sideWall.HeightPx);

            // Guarda el libro de trabajo
            workbook.Save("ChartPropertySideWallDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


