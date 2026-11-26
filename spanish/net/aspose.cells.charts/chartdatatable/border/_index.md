---
title: "ChartDataTable.Border"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartDataTable. Devuelve un objeto Border que representa el borde del objeto"
type: docs
url: /es/net/aspose.cells.charts/chartdatatable/border/
---
## ChartDataTable.Border property

Devuelve un objeto Border que representa el borde del objeto

```csharp
public Line Border { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyBorderDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Mostrar tabla de datos
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Configurar propiedades del borde
            Line border = dataTable.Border;
            border.Color = System.Drawing.Color.Blue;
            border.Style = LineType.Solid;
            border.Weight = WeightType.MediumLine;
            border.DashType = MsoLineDashStyle.Solid;
            
            // Configurar la visibilidad de los bordes de la tabla
            dataTable.HasHorizontalBorder = true;
            dataTable.HasVerticalBorder = true;
            dataTable.HasOutlineBorder = true;

            // Guarda el libro de trabajo
            workbook.Save("ChartDataTableBorderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


