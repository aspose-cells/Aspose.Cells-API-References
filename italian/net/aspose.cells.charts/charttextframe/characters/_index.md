---
title: "ChartTextFrame.Characters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartTextFrame. Restituisce un oggetto Characters che rappresenta un intervallo di caratteri nel testo"
type: docs
url: /it/net/aspose.cells.charts/charttextframe/characters/
---
## ChartTextFrame.Characters method

Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | Int32 | L'indice dell'inizio del carattere. |
| lunghezza | Int32 | Il numero di caratteri. |

### Valore di ritorno

Oggetto Characters.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFrameMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Accedi alle etichette dati e imposta la dimensione del carattere per caratteri specifici
            chart.NSeries[0].Points[0].DataLabels.ShowValue = true;
            chart.NSeries[0].Points[0].DataLabels.Characters(0, 5).Font.Size = 14;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


