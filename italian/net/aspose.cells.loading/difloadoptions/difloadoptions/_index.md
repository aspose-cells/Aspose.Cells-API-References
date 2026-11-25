---
title: "DifLoadOptions.DifLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore DifLoadOptions. Le opzioni"
type: docs
url: /it/net/aspose.cells.loading/difloadoptions/difloadoptions/
---
## DifLoadOptions constructor

Le opzioni.

```csharp
public DifLoadOptions()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DifLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova istanza di DifLoadOptions usando il costruttore senza parametri
                DifLoadOptions loadOptions = new DifLoadOptions();

                // Crea un nuovo workbook con opzioni predefinite
                Workbook workbook = new Workbook();

                // Accedi al primo foglio di lavoro
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi dati di esempio per dimostrare che il workbook è funzionale
                worksheet.Cells["A1"].PutValue("DifLoadOptions Constructor Demo");
                worksheet.Cells["A2"].PutValue("Created at: " + DateTime.Now.ToString());
                worksheet.Cells["A4"].PutValue("This demonstrates using the parameterless constructor");

                // Salva la cartella di lavoro in formato DIF
                workbook.Save("DifLoadOptionsCtorDemo.dif", SaveFormat.Dif);

                // Ora carica il file DIF salvato con DifLoadOptions
                DifLoadOptions difOptions = new DifLoadOptions();
                Workbook loadedWorkbook = new Workbook("DifLoadOptionsCtorDemo.dif", difOptions);

                // Salva i dati caricati in XLSX per verifica
                loadedWorkbook.Save("DifLoadOptionsCtorVerification.xlsx", SaveFormat.Xlsx);

                Console.WriteLine("DifLoadOptions constructor demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DifLoadOptions constructor demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [DifLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


