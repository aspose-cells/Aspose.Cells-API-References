---
title: "Enum PrintSizeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.PrintSizeType enum. Representa el tamaño del gráfico impreso."
type: docs
url: /es/net/aspose.cells/printsizetype/
---
## PrintSizeType enumeration

Representa el tamaño del gráfico impreso.

```csharp
public enum PrintSizeType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Full | `0` | Usar página completa. |
| Fit | `1` | Escalar para ajustar a la página. |
| Custom | `2` | Personalizado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PrintSizeTypeDemo
    {
        public static void PrintSizeTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Obtener la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos para el gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Establecer el título del gráfico
            chart.Title.Text = "Sample Chart";

            // Establecer el tamaño de impresión del gráfico
            chart.PrintSize = PrintSizeType.Fit;

            // Guarda el libro de trabajo
            workbook.Save("PrintSizeTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


