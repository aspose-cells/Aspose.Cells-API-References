---
title: "DataLabels.NumberFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Representa la cadena de formato para el objeto DataLabels"
type: docs
url: /es/net/aspose.cells.charts/datalabels/numberformat/
---
## DataLabels.NumberFormat property

Representa la cadena de formato para el objeto DataLabels.

```csharp
public string NumberFormat { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyNumberFormatDemo
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
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar etiquetas de datos
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Establecer formato numérico personalizado para las etiquetas de datos
            series.DataLabels.NumberFormat = "_(* #,##0_);_(* \\(#,##0\\);_(* \"-\"??_);_(@_)";
            
            // Guarda el libro de trabajo
            workbook.Save("DataLabelsNumberFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


