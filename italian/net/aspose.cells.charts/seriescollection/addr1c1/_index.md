---
title: "SeriesCollection.AddR1C1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SeriesCollection. Aggiunge la collezione Series a un grafico"
type: docs
url: /it/net/aspose.cells.charts/seriescollection/addr1c1/
---
## SeriesCollection.AddR1C1 method

Aggiunge la collezione [`Series`](../../series/) a un grafico.

```csharp
public int AddR1C1(string area, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | String | Specifica i valori da cui tracciare la serie di dati |
| isVertical | Booleano | Specifica se tracciare la serie da un intervallo di valori di cella per riga o per colonna. |

### Valore di ritorno

Restituisce il primo indice della ASeries aggiunta in NSeries.

### Osservazioni

Se i dati sono impostati su celle contigue, utilizzare i due punti per separarle. Per esempio, R[1]C[1]:R[3]C[2]. Se i dati sono impostati su celle contigue, utilizzare la virgola per separarle. Per esempio, (R[1]C[1],R[3]C[2]).

### Esempi

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

            // Dati di esempio
            wsData.Cells[0, 0].PutValue(1);
            wsData.Cells[1, 0].PutValue(2);
            wsData.Cells[0, 1].PutValue(3);
            wsData.Cells[1, 1].PutValue(4);

            Worksheet wsChart = workbook.Worksheets[workbook.Worksheets.Add(Aspose.Cells.SheetType.Chart)];
            wsChart.Name = "ChartSheet";

            int chartIndex = wsChart.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 0, 0, 15, 15);
            Aspose.Cells.Charts.Chart chart = wsChart.Charts[chartIndex];

            // Utilizzo di AddR1C1 con parametri String e Boolean
            int seriesIndex = chart.NSeries.AddR1C1("ChartData!R1C2:R2C2", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.XValues = "ChartData!R1C1:R2C1";

            workbook.Save("SeriesCollectionAddR1C1Demo.xlsx", Aspose.Cells.SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


