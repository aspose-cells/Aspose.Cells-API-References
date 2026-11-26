---
title: "Area.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Area. Devuelve o establece el grado de transparencia del área como un valor de 0.0 opaco a 1.0 transparente"
type: docs
url: /es/net/aspose.cells.drawing/area/transparency/
---
## Area.Transparency property

Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro).

```csharp
public double Transparency { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AreaPropertyTransparencyDemo
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
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder a la primera serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];

            // Demostrar la propiedad Transparency
            Console.WriteLine("Initial area transparency: " + series.Area.Transparency);
            Console.WriteLine("Initial border transparency: " + series.Border.Transparency);

            // Modificar valores de transparencia
            series.Area.Transparency = 0.5; // 50% transparent
            series.Border.Transparency = 0.2; // 20% transparent

            Console.WriteLine("Modified area transparency: " + series.Area.Transparency);
            Console.WriteLine("Modified border transparency: " + series.Border.Transparency);

            // Guarda el libro de trabajo
            workbook.Save("AreaPropertyTransparencyDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


