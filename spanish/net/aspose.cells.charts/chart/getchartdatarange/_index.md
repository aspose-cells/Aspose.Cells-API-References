---
title: "Chart.GetChartDataRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Chart. Obtiene el rango de origen de datos del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/getchartdatarange/
---
## Chart.GetChartDataRange method

Obtiene el rango de origen de datos del gráfico.

```csharp
public string GetChartDataRange()
```

### Valor de retorno

El origen de datos.

### Observaciones

Solo admite rangos. Si Series.Values, Name y XValues están en un rango continuo, se devolverá un rango que los contenga.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodGetChartDataRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C4"].PutValue(60);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("=Sheet1!$B$1:$C$4", true);
            
            // Obtener y mostrar el rango de datos del gráfico
            string dataRange = chart.GetChartDataRange();
            Console.WriteLine("Chart Data Range: " + dataRange);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


