---
title: "ChartDataTable.Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartDataTable. Obtiene un objeto Font que representa la configuración de fuente de la tabla de datos del gráfico especificado"
type: docs
url: /es/net/aspose.cells.charts/chartdatatable/font/
---
## ChartDataTable.Font property

Obtiene un objeto `Font` que representa la configuración de fuente de la tabla de datos del gráfico especificado.

```csharp
public Font Font { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Habilitar tabla de datos
            chart.ShowDataTable = true;
            
            // Obtener el objeto de la tabla de datos
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // Personalizar la fuente de la tabla de datos
            dataTable.Font.Size = 14;
            dataTable.Font.Color = Color.Red;
            dataTable.Font.IsBold = true;
            dataTable.Font.Name = "Arial";

            // Guarda el libro de trabajo
            workbook.Save("ChartDataTableFontDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../../../aspose.cells/font/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


