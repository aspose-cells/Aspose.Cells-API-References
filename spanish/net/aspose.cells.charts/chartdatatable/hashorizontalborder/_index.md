---
title: "ChartDataTable.HasHorizontalBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartDataTable. True si la tabla de datos del gráfico tiene bordes de celda horizontales"
type: docs
url: /es/net/aspose.cells.charts/chartdatatable/hashorizontalborder/
---
## ChartDataTable.HasHorizontalBorder property

Verdadero si la tabla de datos del gráfico tiene bordes horizontales de celda

```csharp
public bool HasHorizontalBorder { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasHorizontalBorderDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar tabla de datos
            chart.ShowDataTable = true;
            // Obtenga la tabla de datos a través de la propiedad ChartDataTable
            ChartDataTable dataTable = chart.ChartDataTable;

            // Demostrar la propiedad HasHorizontalBorder
            dataTable.HasHorizontalBorder = true;
            Console.WriteLine("DataTable HasHorizontalBorder: " + dataTable.HasHorizontalBorder);

            // Guarda el libro de trabajo
            workbook.Save("ChartDataTablePropertyHasHorizontalBorderDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


