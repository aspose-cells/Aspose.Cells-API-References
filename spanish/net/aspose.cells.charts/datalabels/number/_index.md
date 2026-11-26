---
title: "DataLabels.Number"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Obtiene y establece el formato numérico incorporado"
type: docs
url: /es/net/aspose.cells.charts/datalabels/number/
---
## DataLabels.Number property

Obtiene y establece el formato numérico incorporado.

```csharp
public int Number { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyNumberDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Bar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener la primera serie y habilitar las etiquetas de datos
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Acceder a las propiedades de las etiquetas de datos
            DataLabels dataLabels = series.DataLabels;
            
            // Demostrar el uso de la propiedad Number
            Console.WriteLine("Original Number format: " + dataLabels.NumberFormat);
            Console.WriteLine("Original Number property value: " + dataLabels.Number);
            
            // Cambiar el formato numérico
            dataLabels.Number = 2; // Currency format
            dataLabels.NumberFormat = "$#,##0.00";
            
            Console.WriteLine("Modified Number format: " + dataLabels.NumberFormat);
            Console.WriteLine("Modified Number property value: " + dataLabels.Number);

            // Guarda el libro de trabajo
            workbook.Save("DataLabelsNumberDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


