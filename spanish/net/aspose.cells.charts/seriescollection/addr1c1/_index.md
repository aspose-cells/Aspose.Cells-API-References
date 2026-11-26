---
title: "SeriesCollection.AddR1C1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SeriesCollection. Añade la colección Series a un gráfico"
type: docs
url: /es/net/aspose.cells.charts/seriescollection/addr1c1/
---
## SeriesCollection.AddR1C1 method

Añade la colección [`Series`](../../series/) a un gráfico.

```csharp
public int AddR1C1(string area, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| área | String | Especifica los valores a partir de los cuales trazar la serie de datos |
| isVertical | Booleano | Especifica si se debe trazar la serie a partir de un rango de valores de celdas por fila o por columna. |

### Valor de retorno

Devuelve el primer índice de la ASeries añadida en la NSeries.

### Observaciones

Si establece datos en celdas contiguas, use dos puntos para separarlas. Por ejemplo, R[1]C[1]:R[3]C[2]. Si establece datos en celdas contiguas, use coma para separarlas. Por ejemplo, (R[1]C[1],R[3]C[2]).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddR1C1WithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet wsData = workbook.Worksheets[0];
            wsData.Name = "ChartData";

            // Datos de ejemplo
            wsData.Cells[0, 0].PutValue(1);
            wsData.Cells[1, 0].PutValue(2);
            wsData.Cells[0, 1].PutValue(3);
            wsData.Cells[1, 1].PutValue(4);

            Worksheet wsChart = workbook.Worksheets[workbook.Worksheets.Add(Aspose.Cells.SheetType.Chart)];
            wsChart.Name = "ChartSheet";

            int chartIndex = wsChart.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 0, 0, 15, 15);
            Aspose.Cells.Charts.Chart chart = wsChart.Charts[chartIndex];

            // Uso de AddR1C1 con parámetros String y Boolean
            int seriesIndex = chart.NSeries.AddR1C1("ChartData!R1C2:R2C2", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.XValues = "ChartData!R1C1:R2C1";

            workbook.Save("SeriesCollectionAddR1C1Demo.xlsx", Aspose.Cells.SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


