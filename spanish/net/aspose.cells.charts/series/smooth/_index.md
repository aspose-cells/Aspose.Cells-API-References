---
title: "Series.Smooth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Series. Representa el suavizado de curvas. Verdadero si el suavizado de curvas está activado para el gráfico de líneas o de dispersión. Se aplica solo a gráficos de líneas y gráficos de dispersión con líneas"
type: docs
url: /es/net/aspose.cells.charts/series/smooth/
---
## Series.Smooth property

Representa el suavizado de curvas. True si el suavizado de curvas está activado para el gráfico de líneas o de dispersión. Se aplica solo a gráficos de líneas y gráficos de dispersión con líneas.

```csharp
public bool Smooth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySmoothDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer la propiedad Smooth para la primera serie
            chart.NSeries[0].Smooth = true;

            // Guarda el libro de trabajo
            workbook.Save("SmoothPropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


