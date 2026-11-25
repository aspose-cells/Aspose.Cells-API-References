---
title: "Enum SaveElementType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Saving.SaveElementType enum. Rappresenta il tipo di elementi da salvare."
type: docs
url: /it/net/aspose.cells.saving/saveelementtype/
---
## SaveElementType enumeration

Rappresenta quali tipi di elementi devono essere salvati.

```csharp
public enum SaveElementType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| All | `251658239` | Tutti i dati. |
| Chart | `256` | Solo grafici. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassSaveElementTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi alcuni dati di esempio per dimostrare il salvataggio.
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["B1"].PutValue(12345);

                // Crea un grafico per dimostrare il tipo di elemento di salvataggio del grafico.
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B1", true);

                // Dimostra l'uso dei valori dell'enum SaveElementType.
                SaveElementType chartType = SaveElementType.Chart;
                SaveElementType allType = SaveElementType.All;

                Console.WriteLine($"Chart SaveElementType value: {chartType}");
                Console.WriteLine($"All SaveElementType value: {allType}");

                // Salva la cartella di lavoro con tutti gli elementi.
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                workbook.Save("SaveElementTypeDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully with all elements");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SaveElementType: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


