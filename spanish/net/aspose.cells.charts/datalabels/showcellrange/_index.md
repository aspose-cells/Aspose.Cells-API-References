---
title: "DataLabels.ShowCellRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Indica si se debe mostrar el rango de celdas como etiquetas de datos"
type: docs
url: /es/net/aspose.cells.charts/datalabels/showcellrange/
---
## DataLabels.ShowCellRange property

Indica si se muestra el rango de celdas como etiquetas de datos.

```csharp
public bool ShowCellRange { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowCellRangeDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer datos de muestra
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C2"].PutValue("100 units");
            worksheet.Cells["C3"].PutValue("200 units");

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Configurar etiquetas de datos con ShowCellRange
            var series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowCellRange = true;
            series.DataLabels.LinkedSource = "C2:C3";
            series.DataLabels.Font.Color = Color.Blue;

            // Guarda el libro de trabajo
            workbook.Save("DataLabelsShowCellRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


