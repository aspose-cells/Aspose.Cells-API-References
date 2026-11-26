---
title: "Chart.SetChartDataRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método del gráfico. Especifica el rango de datos para un gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/setchartdatarange/
---
## Chart.SetChartDataRange method

Especifica el rango de datos para un gráfico.

```csharp
public void SetChartDataRange(string area, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| área | String | Especifica los valores a partir de los cuales trazar la serie de datos |
| isVertical | Booleano | Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodSetChartDataRangeWithStringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("Cat3");
            worksheet.Cells["B4"].PutValue(30);
            
            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);
            
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


