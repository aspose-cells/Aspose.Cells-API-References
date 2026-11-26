---
title: "Line.BeginArrowLength"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Especifica la longitud de la punta de flecha para el inicio de una línea"
type: docs
url: /es/net/aspose.cells.drawing/line/beginarrowlength/
---
## Line.BeginArrowLength property

Especifica la longitud de la punta de flecha para el inicio de una línea.

```csharp
public MsoArrowheadLength BeginArrowLength { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class LinePropertyBeginArrowLengthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepare datos simples para un gráfico
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

                // Establezca BeginArrowLength a Long
                seriesLine.BeginArrowLength = MsoArrowheadLength.Long;

                // Lea y muestre el valor actual de BeginArrowLength
                Console.WriteLine("BeginArrowLength value: " + seriesLine.BeginArrowLength);

                // Guarda el libro de trabajo (opcional, solo para completar la demostración)
                workbook.Save("BeginArrowLengthDemo.xlsx");
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


