---
title: "Line.GradientFill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Representa el relleno degradado"
type: docs
url: /es/net/aspose.cells.drawing/line/gradientfill/
---
## Line.GradientFill property

Representa el relleno degradado.

```csharp
public GradientFill GradientFill { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;

    public class LinePropertyGradientFillDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo para un gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Obtener el primer punto de la primera serie
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];

            try
            {
                // Acceder al objeto Line (borde) del punto
                Line line = point.Border;

                // Leer la propiedad GradientFill (solo lectura)
                GradientFill gradient = line.GradientFill;

                // Mostrar los detalles actuales del relleno degradado
                Console.WriteLine("Current GradientFill:");
                Console.WriteLine($"  FillType       = {gradient.FillType}");
                Console.WriteLine($"  DirectionType = {gradient.DirectionType}");
                Console.WriteLine($"  Angle          = {gradient.Angle}");

                // Modificar el degradado usando los métodos proporcionados
                // Utilizar una conversión a un valor enum predeterminado para evitar referenciar un miembro inexistente
                gradient.SetGradient(GradientFillType.Linear, 45.0, (GradientDirectionType)0);
                Console.WriteLine("GradientFill after SetGradient:");
                Console.WriteLine($"  Angle = {gradient.Angle}");

                // Guarda el libro de trabajo
                workbook.Save("LinePropertyGradientFillDemo.xlsx");
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

* class [GradientFill](../../gradientfill/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


