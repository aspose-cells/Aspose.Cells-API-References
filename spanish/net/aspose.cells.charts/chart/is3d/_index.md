---
title: "Chart.Is3D"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Indica si el gráfico es un gráfico 3D"
type: docs
url: /es/net/aspose.cells.charts/chart/is3d/
---
## Chart.Is3D property

Indica si el gráfico es un gráfico 3D.

```csharp
public bool Is3D { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyIs3DDemo
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
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos para el gráfico
            chart.SetChartDataRange("A1:B5", true);

            // Mostrar el valor actual de Is3D
            Console.WriteLine("Current Is3D value: " + chart.Is3D);

            // Crear una versión 3D del gráfico
            int chart3DIndex = worksheet.Charts.Add(ChartType.Column3D, 6, 12, 20, 22);
            Chart chart3D = worksheet.Charts[chart3DIndex];
            chart3D.SetChartDataRange("A1:B5", true);

            // Mostrar el valor Is3D del gráfico 3D
            Console.WriteLine("3D Chart Is3D value: " + chart3D.Is3D);

            // Guarda el libro de trabajo
            workbook.Save("ChartPropertyIs3DDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


