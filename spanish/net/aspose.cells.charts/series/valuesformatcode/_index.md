---
title: "Series.ValuesFormatCode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Representa el código de formato de la Values NumberList"
type: docs
url: /es/net/aspose.cells.charts/series/valuesformatcode/
---
## Series.ValuesFormatCode property

Representa el código de formato de la lista de números de Valores.

```csharp
public string ValuesFormatCode { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyValuesFormatCodeDemo
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
            worksheet.Cells["B2"].PutValue(0.25);
            worksheet.Cells["B3"].PutValue(0.5);
            worksheet.Cells["B4"].PutValue(0.75);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer el código de formato de valores para la primera serie
            chart.NSeries[0].ValuesFormatCode = "0.00%";

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertyValuesFormatCodeDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


