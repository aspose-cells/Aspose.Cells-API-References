---
title: "Area.ForegroundColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Area. Obtiene o establece el Color de primer plano"
type: docs
url: /es/net/aspose.cells.drawing/area/foregroundcolor/
---
## Area.ForegroundColor property

Obtiene o establece el Color de primer plano.

```csharp
public Color ForegroundColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyForegroundColorDemo
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

            // Establece diferentes colores de primer plano para cada área de serie
            chart.NSeries[0].Area.ForegroundColor = Color.FromArgb(79, 129, 189);
            chart.NSeries[1].Area.ForegroundColor = Color.FromArgb(192, 80, 77);

            // Guarda el libro de trabajo
            workbook.Save("AreaForegroundColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


