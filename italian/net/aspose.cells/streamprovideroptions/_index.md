---
title: "Classe StreamProviderOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.StreamProviderOptions. Rappresenta le opzioni di flusso"
type: docs
url: /it/net/aspose.cells/streamprovideroptions/
---
## StreamProviderOptions class

Rappresenta le opzioni di flusso.

```csharp
public class StreamProviderOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [StreamProviderOptions](streamprovideroptions/#constructor)() | Inizializza una nuova istanza della classe `StreamProviderOptions`. |
| [StreamProviderOptions](streamprovideroptions/#constructor_1)(ResourceLoadingType, string) | Inizializza una nuova istanza della classe `StreamProviderOptions`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CustomPath](../../aspose.cells/streamprovideroptions/custompath/) { get; set; } | Il percorso personalizzato (URL) dell'utente salvato nel file HTML generato per la fonte di riferimento. Se non definito dall'utente, verrà utilizzato DefaultPath. Ad esempio, i dati del foglio saranno salvati dall'utente in d:/sheet001.htm, l'URL usato nel file HTML principale dovrebbe essere \"d:/sheet001.htm\" o un altro percorso relativo valido che possa essere accessibile dal file HTML principale. |
| [DefaultPath](../../aspose.cells/streamprovideroptions/defaultpath/) { get; } | Il percorso predefinito (URL) salvato nel file html generato per la sorgente di riferimento. Ad esempio, i dati del foglio salvati in xxx_files/sheet001.htm, l'url usato nel file html principale dovrebbe essere così \"src=\\\"xxx_files/sheet001.htm\\\"\" |
| [ResourceLoadingType](../../aspose.cells/streamprovideroptions/resourceloadingtype/) { get; set; } | Ottiene e imposta il tipo di risorsa di caricamento. |
| [Stream](../../aspose.cells/streamprovideroptions/stream/) { get; set; } | Ottiene/Imposta lo stream |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassStreamProviderOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Imposta uno stream di memoria per la dimostrazione
            options.Stream = new MemoryStream();
            
            // Usa lo stream (esempio: salva la cartella di lavoro nello stream)
            workbook.Save(options.Stream, SaveFormat.Xlsx);
            
            // Dimostra la chiusura dello stream
            CloseStream(options);
        }

        public static void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


