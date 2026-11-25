---
title: "ChartCollection.AddFloatingChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartCollection. Aggiunge un grafico alla collezione"
type: docs
url: /it/net/aspose.cells.charts/chartcollection/addfloatingchart/
---
## ChartCollection.AddFloatingChart method

Aggiunge un grafico alla raccolta.

```csharp
public int AddFloatingChart(ChartType type, int left, int top, int width, int height)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ChartType | Tipo di grafico |
| sinistra | Int32 | L'offset x verso l'angolo |
| alto | Int32 | L'offset y verso l'angolo |
| larghezza | Int32 | La larghezza del grafico |
| altezza | Int32 | L'altezza del grafico |

### Valore di ritorno

[`Chart`](../../chart/) object index.

### Esempi

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
            
            // Aggiungi un grafico flottante con le dimensioni specificate
            int chartIndex = sheet.Charts.AddFloatingChart(ChartType.Column, 100, 100, 600, 400);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Aggiungi dati di esempio al grafico
            chart.NSeries.Add("{1,3,2,5}", false);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


