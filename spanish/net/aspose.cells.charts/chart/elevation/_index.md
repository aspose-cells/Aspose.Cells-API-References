---
title: "Chart.Elevation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Representa la elevación de la vista del gráfico 3D en grados"
type: docs
url: /es/net/aspose.cells.charts/chart/elevation/
---
## Chart.Elevation property

Representa la elevación de la vista del gráfico 3-D, en grados.

```csharp
public int Elevation { get; set; }
```

### Observaciones

La elevación del gráfico es la altura a la que se visualiza el gráfico, en grados. El valor predeterminado es 15 para la mayoría de los tipos de gráficos. El valor de esta propiedad debe estar entre -90 y 90, excepto en los gráficos de barras 3D, donde debe estar entre 0 y 44.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyElevationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Agregar un gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer la propiedad de elevación (ángulo en grados)
            chart.Elevation = 30;
            
            // Guarda el libro de trabajo
            workbook.Save("ChartElevationDemo.xlsx");

            Console.WriteLine("Chart created with elevation set to 30 degrees.");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


