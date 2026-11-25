---
title: "Workbook.MergeNamedStyles"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Unisce gli stili denominati dall'altro file Excel"
type: docs
url: /it/net/aspose.cells/workbook/mergenamedstyles/
---
## Workbook.MergeNamedStyles method

Unisce gli stili denominati dall'altro file Excel.

```csharp
public void MergeNamedStyles(Workbook source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Cartella di lavoro | L'altro file |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodMergeNamedStylesWithWorkbookDemo
    {
        public static void Run()
        {
            // Crea la cartella di lavoro di destinazione (quella che riceverà gli stili denominati)
            using (Workbook targetWorkbook = new Workbook())
            {
                // Aggiungi alcuni dati alla cartella di lavoro di destinazione per fornire contesto
                Worksheet targetSheet = targetWorkbook.Worksheets[0];
                targetSheet.Cells["A1"].PutValue("Target Workbook");

                // Crea la cartella di lavoro di origine (quella che contiene gli stili denominati da unire)
                using (Workbook sourceWorkbook = new Workbook())
                {
                    // Aggiungi alcuni dati alla cartella di lavoro di origine per fornire contesto
                    Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
                    sourceSheet.Cells["A1"].PutValue("Source Workbook");

                    try
                    {
                        // Unisci gli stili denominati da sourceWorkbook in targetWorkbook
                        targetWorkbook.MergeNamedStyles(sourceWorkbook);

                        Console.WriteLine("MergeNamedStyles executed successfully.");

                        // Salva la cartella di lavoro risultante
                        string outputPath = "MergedNamedStylesDemo.xlsx";
                        targetWorkbook.Save(outputPath, SaveFormat.Xlsx);
                        Console.WriteLine($"Workbook saved to '{outputPath}'.");
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine($"Error during MergeNamedStyles: {ex.Message}");
                    }
                }
            }
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


