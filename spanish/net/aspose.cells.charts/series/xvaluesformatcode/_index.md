---
title: "Series.XValuesFormatCode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Series. Representa el código de formato de la lista de números de valores X"
type: docs
url: /es/net/aspose.cells.charts/series/xvaluesformatcode/
---
## Series.XValuesFormatCode property

Representa el código de formato de la lista de números de Valores X.

```csharp
public string XValuesFormatCode { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesFormatCodeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B3"].PutValue(200);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Establecer el código de formato de XValues
            chart.NSeries[0].XValuesFormatCode = "M/d/yyyy";

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertyXValuesFormatCodeDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


