---
title: "Chart.IsRectangularCornered"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Chart property. Obtiene o establece un valor que indica si el área del gráfico tiene esquinas rectangulares. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells.charts/chart/isrectangularcornered/
---
## Chart.IsRectangularCornered property

Obtiene o establece un valor que indica si el área del gráfico tiene esquinas rectangulares. El valor predeterminado es true.

```csharp
public bool IsRectangularCornered { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyIsRectangularCorneredDemo
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
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demostrar la propiedad IsRectangularCornered
            Console.WriteLine("Default IsRectangularCornered: " + chart.IsRectangularCornered);
            
            // Establecer en true para que las esquinas del gráfico sean rectangulares
            chart.IsRectangularCornered = true;
            Console.WriteLine("After setting IsRectangularCornered to true: " + chart.IsRectangularCornered);

            // Guarda el libro de trabajo
            workbook.Save("ChartPropertyIsRectangularCorneredDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


