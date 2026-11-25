---
title: "Classe AbstractLowCodeLoadOptionsProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LowCode.AbstractLowCodeLoadOptionsProvider. Implementazione per fornire opzioni di caricamento multiple per processi che utilizzano più input, come i file modello"
type: docs
url: /it/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/
---
## AbstractLowCodeLoadOptionsProvider class

Implementazione per fornire più opzioni di caricamento per i processi che utilizzano più input (come i file modello).

```csharp
public abstract class AbstractLowCodeLoadOptionsProvider
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| abstract [Current](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/) { get; } | Ottiene le opzioni di caricamento da cui caricare i dati della parte attualmente elaborata. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/)(LowCodeLoadOptions) | Rilascia le risorse dopo aver elaborato la parte corrente dell'input. |
| abstract [MoveNext](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/)() | Verifica se ci sono ulteriori dati in input. |

### Osservazioni

Ad esempio, la funzionalità [`SpreadsheetMerger`](../spreadsheetmerger/) richiede più file modello da unire.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Crea un'implementazione personalizzata di AbstractLowCodeLoadOptionsProvider
            var provider = new CustomLoadOptionsProvider();

            // Elabora più input utilizzando il provider
            while (provider.MoveNext())
            {
                // Ottieni le opzioni di caricamento correnti
                LowCodeLoadOptions currentOptions = provider.Current;
                Console.WriteLine($"Processing with load options: {currentOptions}");

                // Crea una cartella di lavoro con le opzioni correnti
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                Worksheet worksheet = workbook.Worksheets[0];

                // Dimostra l'uso con la cartella di lavoro
                worksheet.Cells["A1"].PutValue("Processed with custom provider");
                
                // Completa l'elaborazione di questa parte
                provider.Finish(currentOptions);
            }
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int currentIndex = 0;
            private readonly LowCodeLoadOptions[] optionsList = new LowCodeLoadOptions[]
            {
                new LowCodeLoadOptions(),
                new LowCodeLoadOptions { InputFile = "protected.xlsx" }, // Password would be handled separately
                new LowCodeLoadOptions() // MemorySetting would be handled separately
            };

            public override LowCodeLoadOptions Current => optionsList[currentIndex];

            public override bool MoveNext()
            {
                if (currentIndex < optionsList.Length - 1)
                {
                    currentIndex++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // Logica di pulizia o finalizzazione per ogni parte
                Console.WriteLine($"Finished processing part {currentIndex}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


