---
title: "Line.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Devuelve o establece el grado de transparencia de la línea como un valor de 0.0 opaco a 1.0 claro"
type: docs
url: /es/net/aspose.cells.drawing/line/transparency/
---
## Line.Transparency property

Devuelve o establece el grado de transparencia de la línea como un valor de 0.0 (opaco) a 1.0 (claro).

```csharp
public double Transparency { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para que el ejemplo tenga sentido
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            try
            {
                // Agregar un gráfico de líneas para demostrar las propiedades de la línea
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Obtener las propiedades de la línea del borde de la serie del gráfico
                Line line = chart.NSeries[0].Border;

                // Mostrar el valor actual de Transparency
                Console.WriteLine("Current Transparency: " + line.Transparency);

                // Establecer un nuevo valor de Transparency (0.0 = opaco, 1.0 = claro)
                line.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + line.Transparency);

                // Guarda el libro de trabajo
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("Transparency property demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


