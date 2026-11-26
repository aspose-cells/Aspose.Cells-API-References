---
title: "Line.EndArrowLength"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Especifica la longitud de la punta de flecha para el extremo de una línea"
type: docs
url: /es/net/aspose.cells.drawing/line/endarrowlength/
---
## Line.EndArrowLength property

Especifica la longitud de la punta de flecha para el final de una línea.

```csharp
public MsoArrowheadLength EndArrowLength { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyEndArrowLengthDemo
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
                // Añadir un gráfico para demostrar las propiedades de la línea
                int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Obtener las propiedades de la línea del borde de la serie del gráfico
                Line line = chart.NSeries[0].Border;

                // Establecer un tipo de punta de flecha para demostrar EndArrowLength
                line.EndType = MsoArrowheadStyle.Arrow;

                // Mostrar el valor actual de EndArrowLength
                Console.WriteLine("Current EndArrowLength: " + line.EndArrowLength);

                // Establecer un nuevo valor de EndArrowLength
                line.EndArrowLength = MsoArrowheadLength.Long;
                Console.WriteLine("Updated EndArrowLength: " + line.EndArrowLength);

                // Guarda el libro de trabajo
                workbook.Save("EndArrowLengthDemo.xlsx");
                Console.WriteLine("EndArrowLength property demonstrated successfully.");
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

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


