---
title: "Area.BackgroundColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Area. Obtiene o establece el Color de fondo del Area"
type: docs
url: /es/net/aspose.cells.drawing/area/backgroundcolor/
---
## Area.BackgroundColor property

Obtiene o establece el Color de fondo del [`Area`](../).

```csharp
public Color BackgroundColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Establece el color de fondo para el área del eje de categoría
            chart.CategoryAxis.Area.BackgroundColor = System.Drawing.Color.Red;

            // Muestra el color de fondo
            Console.WriteLine("Category Axis Background Color: " + chart.CategoryAxis.Area.BackgroundColor);

            // Guarda el libro de trabajo
            workbook.Save("AreaPropertyBackgroundColorDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


