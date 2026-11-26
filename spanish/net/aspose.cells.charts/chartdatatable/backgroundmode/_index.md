---
title: "ChartDataTable.BackgroundMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartDataTable. Obtiene y establece el modo de visualización del fondo"
type: docs
url: /es/net/aspose.cells.charts/chartdatatable/backgroundmode/
---
## ChartDataTable.BackgroundMode property

Obtiene y establece el modo de visualización del fondo

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyBackgroundModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurar tabla de datos
            chart.ShowDataTable = true;
            ChartDataTable chartTable = chart.ChartDataTable;
            
            // Demostrar el uso de BackgroundMode
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.Font.Color = Color.Blue;
            chartTable.HasBorderOutline = true;

            workbook.Save("ChartDataTableBackgroundModeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


