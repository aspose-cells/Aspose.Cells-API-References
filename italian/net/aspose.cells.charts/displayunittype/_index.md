---
title: "Enum DisplayUnitType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.DisplayUnitType enum. Rappresenta il tipo di unità di visualizzazione dell'asse dei grafici"
type: docs
url: /it/net/aspose.cells.charts/displayunittype/
---
## DisplayUnitType enumeration

Rappresenta il tipo di unità di visualizzazione dell'asse del grafico.

```csharp
public enum DisplayUnitType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | L'unità di visualizzazione è Nessuna. |
| Hundreds | `1` | Specifica che i valori del grafico devono essere divisi per 100. |
| Thousands | `2` | Specifica che i valori del grafico devono essere divisi per 1,000. |
| TenThousands | `3` | Specifica che i valori del grafico devono essere divisi per 10,000. |
| HundredThousands | `4` | Specifica che i valori del grafico devono essere divisi per 100,000. |
| Millions | `5` | Specifica che i valori del grafico devono essere divisi per 1,000,000. |
| TenMillions | `6` | Specifica che i valori del grafico devono essere divisi per 10,000,000. |
| HundredMillions | `7` | Specifica che i valori del grafico devono essere divisi per 100,000,000. |
| Billions | `8` | Specifica che i valori del grafico devono essere divisi per 1,000,000,000. |
| Trillions | `9` | Specifica che i valori del grafico devono essere divisi per 1,000,000,000,000. |
| Percentage | `10` | I valori del grafico devono essere divisi per 0,01. |
| Cust | `11` | Specifica un valore personalizzato per l'unità di visualizzazione. |
| Custom | `12` | Specifica un valore personalizzato per l'unità di visualizzazione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitTypeDemo
    {
        public static void DisplayUnitTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Imposta l'unità di visualizzazione dell'asse dei valori su Milioni
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            
            // Facoltativamente, mostra l'etichetta dell'unità di visualizzazione
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Salva la cartella di lavoro
            workbook.Save("DisplayUnitTypeExample.xlsx");
            workbook.Save("DisplayUnitTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


