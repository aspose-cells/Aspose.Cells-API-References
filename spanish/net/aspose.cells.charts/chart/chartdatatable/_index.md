---
title: "Chart.ChartDataTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Representa la tabla de datos del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/chartdatatable/
---
## Chart.ChartDataTable property

Representa la tabla de datos del gráfico.

```csharp
public ChartDataTable ChartDataTable { get; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyChartDataTableDemo
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
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";

            // Habilitar y personalizar la tabla de datos
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Establecer propiedades de la tabla de datos
            dataTable.ShowLegendKey = true;
            dataTable.HasBorderHorizontal = true;
            dataTable.HasBorderVertical = true;
            dataTable.HasBorderOutline = true;
            dataTable.AutoScaleFont = true;
            dataTable.BackgroundMode = BackgroundMode.Opaque;

            // Personalizar la fuente de la tabla de datos
            dataTable.Font.Name = "Arial";
            dataTable.Font.Size = 10;
            dataTable.Font.Color = Color.Blue;
            dataTable.Font.IsBold = true;

            // Personalizar los bordes de la tabla de datos
            dataTable.Border.Color = Color.Red;
            dataTable.Border.Style = LineType.Dash;
            dataTable.Border.Weight = WeightType.MediumLine;

            // Guarda el libro de trabajo
            workbook.Save("ChartDataTableDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartDataTable](../../chartdatatable/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


