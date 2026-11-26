---
title: "ChartCollection.AddFloatingChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartCollection. Agrega un gráfico a la colección"
type: docs
url: /es/net/aspose.cells.charts/chartcollection/addfloatingchart/
---
## ChartCollection.AddFloatingChart method

Añade un gráfico a la colección.

```csharp
public int AddFloatingChart(ChartType type, int left, int top, int width, int height)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ChartType | Tipo de gráfico |
| izquierda | Int32 | El desplazamiento x al rincón |
| superior | Int32 | El desplazamiento y al rincón |
| ancho | Int32 | El ancho del gráfico |
| altura | Int32 | La altura del gráfico |

### Valor de retorno

[`Chart`](../../chart/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddFloatingChartWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar gráfico flotante con dimensiones especificadas
            int chartIndex = sheet.Charts.AddFloatingChart(ChartType.Column, 100, 100, 600, 400);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Agregar datos de muestra al gráfico
            chart.NSeries.Add("{1,3,2,5}", false);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


