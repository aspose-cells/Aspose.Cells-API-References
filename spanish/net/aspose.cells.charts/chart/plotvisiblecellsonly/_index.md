---
title: "Chart.PlotVisibleCellsOnly"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Chart property. Indica si solo se trazan las celdas visibles"
type: docs
url: /es/net/aspose.cells.charts/chart/plotvisiblecellsonly/
---
## Chart.PlotVisibleCellsOnly property

Indica si solo se trazan celdas visibles del gráfico.

```csharp
public bool PlotVisibleCellsOnly { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotVisibleCellsOnlyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);
            
            // Ocultar fila 3
            worksheet.Cells.Rows[2].IsHidden = true;
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Establecer PlotVisibleCellsOnly a false (el valor predeterminado es true)
            chart.PlotVisibleCellsOnly = false;
            
            // Guarda el libro de trabajo
            workbook.Save("ChartPlotVisibleCellsOnlyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


