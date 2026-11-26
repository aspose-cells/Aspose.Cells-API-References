---
title: "Enumeración BubbleSizeRepresents"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.BubbleSizeRepresents enum. Representa lo que el tamaño de la burbuja indica en un gráfico de burbujas."
type: docs
url: /es/net/aspose.cells.charts/bubblesizerepresents/
---
## BubbleSizeRepresents enumeration

Representa lo que el tamaño de la burbuja indica en un gráfico de burbujas.

```csharp
public enum BubbleSizeRepresents
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| SizeIsArea | `0` | Representa el valor de [`BubbleSizes`](../series/bubblesizes/), que es el área de la burbuja. |
| SizeIsWidth | `1` | Representa el valor de [`BubbleSizes`](../series/bubblesizes/), que es el ancho de la burbuja. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class BubbleSizeRepresentsDemo
    {
        public static void BubbleSizeRepresentsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico de burbujas
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["C1"].PutValue(5);
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);

            // Agregar un gráfico de burbujas a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar series al gráfico de burbujas
            int seriesIndex = chart.NSeries.Add("A1:C3", true);
            Series series = chart.NSeries[seriesIndex];

            // Establecer los valores X, los valores Y y los tamaños de las burbujas
            series.XValues = "A1:A3";
            series.Values = "B1:B3";
            series.BubbleSizes = "C1:C3";

            // Establecer la representación del tamaño de la burbuja
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Guarda el libro de trabajo
            workbook.Save("BubbleSizeRepresentsExample.xlsx");
            workbook.Save("BubbleSizeRepresentsExample.pdf");

            // Establecer la representación del tamaño de la burbuja
            series.SizeRepresents = BubbleSizeRepresents.SizeIsWidth;

            // Guarda el libro de trabajo
            workbook.Save("BubbleSizeRepresentsExample2.xlsx");
            workbook.Save("BubbleSizeRepresentsExample2.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


