---
title: "Chart.SetChartDataRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Chart. Specifica l'intervallo di dati per un grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/setchartdatarange/
---
## Chart.SetChartDataRange method

Specifica l'intervallo di dati per un grafico.

```csharp
public void SetChartDataRange(string area, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | String | Specifica i valori da cui tracciare la serie di dati |
| isVertical | Booleano | Specifica se tracciare la serie da un intervallo di valori di cella per riga o per colonna. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("Cat3");
            worksheet.Cells["B4"].PutValue(30);
            
            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


