---
title: "Series.SplitValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Devuelve o establece un valor que se usará para determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel"
type: docs
url: /es/net/aspose.cells.charts/series/splitvalue/
---
## Series.SplitValue property

Devuelve o establece un valor que se utilizará para determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel.

```csharp
public double SplitValue { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySplitValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grape");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);
            worksheet.Cells["B5"].PutValue(50);

            // Agregar un gráfico de pastel
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Establecer tipo y valor de división
            chart.NSeries[0].SplitType = ChartSplitType.Custom;
            chart.NSeries[0].SplitValue = 20; // Split points with value <= 20

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertySplitValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


