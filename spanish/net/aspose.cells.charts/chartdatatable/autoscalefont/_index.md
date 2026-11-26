---
title: "ChartDataTable.AutoScaleFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartDataTable. Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. El valor predeterminado es Verdadero"
type: docs
url: /es/net/aspose.cells.charts/chartdatatable/autoscalefont/
---
## ChartDataTable.AutoScaleFont property

True si el texto en el objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor predeterminado es True.

```csharp
public bool AutoScaleFont { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyAutoScaleFontDemo
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

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar tabla de datos
            chart.ShowDataTable = true;
            
            // Acceder a las propiedades de la tabla de datos del gráfico
            // Forma correcta de obtener ChartDataTable cuando ShowDataTable es verdadero
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // Demostrar la propiedad AutoScaleFont
            dataTable.AutoScaleFont = false; // Disable auto-scaling
            Console.WriteLine("AutoScaleFont (false): " + dataTable.AutoScaleFont);
            
            dataTable.AutoScaleFont = true; // Enable auto-scaling
            Console.WriteLine("AutoScaleFont (true): " + dataTable.AutoScaleFont);

            // Guarda el libro de trabajo
            workbook.Save("ChartDataTableAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


