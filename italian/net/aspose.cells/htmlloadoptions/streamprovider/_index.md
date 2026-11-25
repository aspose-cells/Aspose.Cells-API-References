---
title: "HtmlLoadOptions.StreamProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlLoadOptions. Ottiene o imposta lo StreamProviderImportHtmlFile per l'importazione di oggetti"
type: docs
url: /it/net/aspose.cells/htmlloadoptions/streamprovider/
---
## HtmlLoadOptions.StreamProvider property

Ottiene o imposta lo StreamProviderImportHtmlFile per l'importazione di oggetti.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyStreamProviderDemo : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            // Inizializza lo stream secondo necessità
        }

        public Stream ProvideStream(StreamProviderOptions options)
        {
            // Restituisce uno stream per lettura/scrittura
            return File.Open(options.DefaultPath, FileMode.OpenOrCreate, FileAccess.ReadWrite);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Chiudi lo stream
            options.Stream.Close();
        }

        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("StreamProvider Demo");

            // Salva con StreamProvider personalizzato
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
            workbook.Save("output.html", saveOptions);

            // Carica con StreamProvider personalizzato
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("output.html", loadOptions);

            // Verifica i dati caricati
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Vedi anche

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


