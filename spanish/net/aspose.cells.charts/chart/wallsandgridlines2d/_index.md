---
title: "Chart.WallsAndGridlines2D"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Verdadero si las líneas de cuadrícula se dibujan bidimensionalmente en un gráfico 3D"
type: docs
url: /es/net/aspose.cells.charts/chart/wallsandgridlines2d/
---
## Chart.WallsAndGridlines2D property

True si las líneas de cuadrícula se dibujan bidimensionalmente en un gráfico 3-D.

```csharp
public bool WallsAndGridlines2D { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyWallsAndGridlines2DDemo
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
            worksheet.Cells["B4"].PutValue(15);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demostrar la propiedad WallsAndGridlines2D
            chart.WallsAndGridlines2D = true; // Show walls and gridlines in 2D
            Console.WriteLine("WallsAndGridlines2D is set to: " + chart.WallsAndGridlines2D);

            // Guarda el libro de trabajo
            workbook.Save("WallsAndGridlines2DDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


