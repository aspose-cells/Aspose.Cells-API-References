---
title: "ChartDataTable.HasBorderOutline"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartDataTable. Verdadero si la tabla de datos del gráfico tiene bordes de contorno"
type: docs
url: /es/net/aspose.cells.charts/chartdatatable/hasborderoutline/
---
## ChartDataTable.HasBorderOutline property

Verdadero si la tabla de datos del gráfico tiene bordes de contorno

```csharp
[Obsolete("Use ChartDataTable.HasOutlineBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderOutline { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ChartDataTable.HasOutlineBorder. Esta propiedad será eliminada 12 meses después desde junio de 2024. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasBorderOutlineDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Habilitar y configurar la tabla de datos
            chart.ShowDataTable = true;
            ChartDataTable chartTable = chart.ChartDataTable;
            
            // Demostrar la propiedad HasBorderOutline
            chartTable.HasBorderOutline = true;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.Font.Color = Color.Blue;

            workbook.Save("ChartDataTableWithBorderOutline.xlsx");
        }
    }
}
```

### Ver también

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


