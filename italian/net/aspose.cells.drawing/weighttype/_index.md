---
title: "Enum WeightType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.WeightType enum. Elenca i tipi di spessore per un bordo immagine o una linea di grafico"
type: docs
url: /it/net/aspose.cells.drawing/weighttype/
---
## WeightType enumeration

Enumera i tipi di spessore per il bordo di un'immagine o per una linea di grafico.

```csharp
public enum WeightType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| HairLine | `-1` | Rappresenta lo spessore di una linea sottile. |
| MediumLine | `1` | Rappresenta lo spessore di una linea media. |
| SingleLine | `0` | Rappresenta lo spessore di una linea singola. |
| WideLine | `2` | Rappresenta lo spessore di una linea larga. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassWeightTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un grafico e ottieni la sua area del grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // Imposta il tipo di spessore del bordo
            chartArea.Border.Weight = WeightType.WideLine;
            
            // Verifica il tipo di spessore
            Console.WriteLine("Chart Area Border Weight: " + chartArea.Border.Weight);
            
            // Salva la cartella di lavoro
            workbook.Save("WeightTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


