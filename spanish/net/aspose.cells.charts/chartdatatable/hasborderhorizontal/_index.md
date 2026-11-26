---
title: "ChartDataTable.HasBorderHorizontal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartDataTable. True si la tabla de datos del gráfico tiene bordes de celda horizontales"
type: docs
url: /es/net/aspose.cells.charts/chartdatatable/hasborderhorizontal/
---
## ChartDataTable.HasBorderHorizontal property

Verdadero si la tabla de datos del gráfico tiene bordes horizontales de celda

```csharp
[Obsolete("Use ChartDataTable.HasHorizontalBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderHorizontal { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad ChartDataTable.HasHorizontalBorder. Esta propiedad será eliminada 12 meses después a partir de junio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasBorderHorizontalDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.ShowDataTable = true;

            ChartDataTable chartTable = chart.ChartDataTable;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = false;
            chartTable.HasBorderOutline = false;

            workbook.Save("ChartDataTable_HasBorderHorizontal.xlsx");
        }
    }
}
```

### Ver también

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


