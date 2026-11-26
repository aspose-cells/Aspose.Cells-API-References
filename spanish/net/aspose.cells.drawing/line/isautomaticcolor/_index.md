---
title: "Line.IsAutomaticColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Indica si el color de la línea se asigna automáticamente"
type: docs
url: /es/net/aspose.cells.drawing/line/isautomaticcolor/
---
## Line.IsAutomaticColor property

Indica si el color de la línea se asigna automáticamente.

```csharp
public bool IsAutomaticColor { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LinePropertyIsAutomaticColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para un gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Agregar un gráfico de líneas
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Acceder a la línea (borde) de la primera serie
                Line seriesLine = chart.NSeries[0].Border;

                // Leer y mostrar el valor de la propiedad IsAutomaticColor
                Console.WriteLine("IsAutomaticColor value: " + seriesLine.IsAutomaticColor);

                // Guarda el libro de trabajo
                workbook.Save("IsAutomaticColorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


