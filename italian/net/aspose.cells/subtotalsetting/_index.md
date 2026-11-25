---
title: "Class SubtotalSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.SubtotalSetting. Rappresenta l'impostazione del subtotale"
type: docs
url: /it/net/aspose.cells/subtotalsetting/
---
## SubtotalSetting class

Rappresenta l'impostazione del subtotale.

```csharp
public class SubtotalSetting
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [GroupBy](../../aspose.cells/subtotalsetting/groupby/) { get; } | Il campo per il raggruppamento, come offset intero a base zero |
| [SubtotalFunction](../../aspose.cells/subtotalsetting/subtotalfunction/) { get; } | La funzione di subtotale. |
| [SummaryBelowData](../../aspose.cells/subtotalsetting/summarybelowdata/) { get; } | Indica se aggiungere il riepilogo sotto i dati. |
| [TotalList](../../aspose.cells/subtotalsetting/totallist/) { get; } | Un array di offset di campo basati su zero, che indica i campi a cui vengono aggiunti i subtotali. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSubtotalSettingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi dati di esempio al foglio di lavoro
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("Group A");
                worksheet.Cells["A3"].PutValue("Group B");
                worksheet.Cells["A4"].PutValue("Group A");
                worksheet.Cells["A5"].PutValue("Group B");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);
                worksheet.Cells["B4"].PutValue(300);
                worksheet.Cells["B5"].PutValue(400);

                // Definisci l'area della cella per i subtotali
                CellArea area = CellArea.CreateCellArea("A1", "B5");

                // Applica i subtotali ai dati
                worksheet.Cells.Subtotal(
                    area,
                    0, // Group by first column (Category)
                    ConsolidationFunction.Sum,
                    new int[] { 1 }, // Subtotal on second column (Value)
                    true,
                    true,
                    true);

                // Recupera il SubtotalSetting dal foglio di lavoro
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Visualizza le proprietà del SubtotalSetting
                Console.WriteLine("Subtotal Setting Properties:");
                Console.WriteLine($"GroupBy field index: {subtotalSetting.GroupBy}");
                Console.WriteLine($"Subtotal Function: {subtotalSetting.SubtotalFunction}");
                Console.WriteLine($"TotalList contains column index: {subtotalSetting.TotalList[0]}");
                Console.WriteLine($"Summary Below Data: {subtotalSetting.SummaryBelowData}");

                // Salva la cartella di lavoro
                workbook.Save("SubtotalSettingDemo.xlsx");
                Console.WriteLine("SubtotalSetting demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SubtotalSetting: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


