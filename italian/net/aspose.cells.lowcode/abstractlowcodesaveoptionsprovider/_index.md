---
title: "Classe AbstractLowCodeSaveOptionsProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider. Implementazione per fornire più opzioni di salvataggio per processi che richiedono più output. Ad esempio, la funzionalità SpreadsheetSplitter richiede più destinazioni per salvare i file divisi"
type: docs
url: /it/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/
---
## AbstractLowCodeSaveOptionsProvider class

Implementazione per fornire più opzioni di salvataggio per processi che richiedono più output. Ad esempio, la funzionalità [`SpreadsheetSplitter`](../spreadsheetsplitter/) richiede più destinazioni per salvare i file divisi.

```csharp
public abstract class AbstractLowCodeSaveOptionsProvider
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Rilascia le risorse dopo l'elaborazione della parte attualmente divisa. |
| abstract [GetSaveOptions](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/)(SplitPartInfo) | Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte attualmente divisa. Restituire null indica di saltare la parte fornita. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeSaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Crea un provider personalizzato estendendo AbstractLowCodeSaveOptionsProvider
            var customProvider = new CustomSaveOptionsProvider();

            // Crea una cartella di lavoro e un foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola alcuni dati
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // Crea le informazioni della parte divisa - in un utilizzo reale, provengono dall'API
            // Poiché non possiamo costruirlo direttamente, passeremo semplicemente null a scopo dimostrativo
            SplitPartInfo splitPartInfo = null;
            
            // Ottieni le opzioni di salvataggio dal provider
            LowCodeSaveOptions saveOptions = customProvider.GetSaveOptions(splitPartInfo);
            
            // Configura le opzioni di salvataggio (esempio)
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            
            // Dimostra il completamento del processo
            customProvider.Finish(saveOptions);
            
            // Salva la cartella di lavoro (non direttamente correlato al provider, solo per dimostrazione)
            workbook.Save("LowCodeSaveOptionsDemo.xlsx");
        }
    }

    // Implementazione personalizzata di AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Crea e restituisci opzioni di salvataggio personalizzate basate sulle informazioni della parte
            return new LowCodeSaveOptions()
            {
                SaveFormat = SaveFormat.Xlsx
                // Rimosso CachedFileFolder poiché non esiste in LowCodeSaveOptions
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Logica di pulizia o finalizzazione qui
            Console.WriteLine("Save operation completed for part");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


