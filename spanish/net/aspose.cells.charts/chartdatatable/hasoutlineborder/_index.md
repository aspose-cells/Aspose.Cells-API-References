---
title: "ChartDataTable.HasOutlineBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartDataTable. Verdadero si la tabla de datos del gráfico tiene bordes de contorno"
type: docs
url: /es/net/aspose.cells.charts/chartdatatable/hasoutlineborder/
---
## ChartDataTable.HasOutlineBorder property

Verdadero si la tabla de datos del gráfico tiene bordes de contorno

```csharp
public bool HasOutlineBorder { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasOutlineBorderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Mostrar la tabla de datos y obtener el objeto ChartDataTable
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Demostrar la propiedad HasOutlineBorder
            dataTable.HasOutlineBorder = true; // Enable outline border
            Console.WriteLine("DataTable HasOutlineBorder: " + dataTable.HasOutlineBorder);

            // Guarda el libro de trabajo
            workbook.Save("ChartDataTableHasOutlineBorderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


