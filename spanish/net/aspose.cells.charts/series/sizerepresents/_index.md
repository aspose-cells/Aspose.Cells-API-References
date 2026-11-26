---
title: "Series.SizeRepresents"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene o establece lo que representa el tamaño de la burbuja en un gráfico de burbujas"
type: docs
url: /es/net/aspose.cells.charts/series/sizerepresents/
---
## Series.SizeRepresents property

Obtiene o establece lo que representa el tamaño de la burbuja en un gráfico de burbujas.

```csharp
public BubbleSizeRepresents SizeRepresents { get; set; }
```

### Observaciones

BubbleSizeRepresents.SizeIsArea indica que el valor [`BubbleSizes`](../bubblesizes/) es el área de la burbuja. BubbleSizeRepresents.SizeIsWidth indica que el valor [`BubbleSizes`](../bubblesizes/) es el ancho de la burbuja.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySizeRepresentsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico de burbujas
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["C1"].PutValue("Size");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
                sheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Agregar un gráfico de burbujas
            int chartIndex = sheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Establecer datos de la serie
            SeriesCollection series = chart.NSeries;
            series.Add("B2:B5", true);
            series.CategoryData = "A2:A5";
            series[0].BubbleSizes = "C2:C5";

            // Establecer la propiedad SizeRepresents
            series[0].SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertySizeRepresentsDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [BubbleSizeRepresents](../../bubblesizerepresents/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


