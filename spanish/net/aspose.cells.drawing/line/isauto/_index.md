---
title: "Line.IsAuto"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Indica si este estilo de línea se asigna automáticamente"
type: docs
url: /es/net/aspose.cells.drawing/line/isauto/
---
## Line.IsAuto property

Indica si este estilo de línea se asigna automáticamente.

```csharp
public bool IsAuto { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyIsAutoDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Agregar un gráfico de líneas
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

                // Establecer rango de datos del gráfico
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Acceder a las propiedades de línea de la serie
                Aspose.Cells.Charts.Series series = chart.NSeries[0];
                Line line = series.Border;

                // Mostrar el valor actual de IsAuto
                Console.WriteLine("Initial IsAuto value: " + line.IsAuto);

                // Establecer IsAuto a true
                line.IsAuto = true;
                Console.WriteLine("After setting to true, IsAuto value: " + line.IsAuto);

                // Establecer IsAuto a false
                line.IsAuto = false;
                Console.WriteLine("After setting to false, IsAuto value: " + line.IsAuto);

                // Guarda el libro de trabajo
                workbook.Save("IsAutoDemo.xlsx");
                Console.WriteLine("IsAuto property has been demonstrated successfully.");
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


