---
title: "StreamProviderOptions.CustomPath"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StreamProviderOptions. L'URL del percorso personalizzato dell'utente salvato nel file HTML generato per la fonte di riferimento. Se non definito dall'utente, verrà usato DefaultPath. Per esempio, i dati del foglio saranno salvati dall'utente in d/sheet001.htm; l'URL usato nel file HTML principale dovrebbe essere d/sheet001.htm o un altro percorso relativo valido che possa essere accessibile dal file HTML principale."
type: docs
url: /it/net/aspose.cells/streamprovideroptions/custompath/
---
## StreamProviderOptions.CustomPath property

Il percorso personalizzato (URL) dell'utente salvato nel file HTML generato per la fonte di riferimento. Se non definito dall'utente, verrà utilizzato DefaultPath. Ad esempio, i dati del foglio saranno salvati dall'utente in d:/sheet001.htm, l'URL usato nel file HTML principale dovrebbe essere \"d:/sheet001.htm\" o un altro percorso relativo valido che possa essere accessibile dal file HTML principale.

```csharp
public string CustomPath { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyCustomPathDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Configura le opzioni di salvataggio HTML con un provider di stream personalizzato
            string outputDir = "output";
            Directory.CreateDirectory(outputDir);
            
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
            
            // Crea provider di stream personalizzato con CustomPath
            HtmlWithExternalResourcesProvider streamProvider = new HtmlWithExternalResourcesProvider(outputDir);
            streamProvider.streamProviderOptions.CustomPath = "resources";
            options.StreamProvider = streamProvider;

            // Salva la cartella di lavoro
            string outputFile = Path.Combine(outputDir, "output.html");
            workbook.Save(outputFile, options);

            // Verifica che il percorso personalizzato sia stato utilizzato
            string resourcePath = Path.Combine(outputDir, streamProvider.streamProviderOptions.CustomPath);
            Console.WriteLine($"Resources should be saved to: {resourcePath}");
        }
    }

    // Implementazione semplificata del provider di stream personalizzato
    public class HtmlWithExternalResourcesProvider : IStreamProvider
    {
        public StreamProviderOptions streamProviderOptions = new StreamProviderOptions();
        public string _outputDirectory;

        public HtmlWithExternalResourcesProvider(string outputDirectory)
        {
            _outputDirectory = outputDirectory;
        }

        public void InitStream(StreamProviderOptions options)
        {
            // L'implementazione andrebbe inserita qui
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // L'implementazione andrebbe inserita qui
        }
    }
}
```

### Vedi anche

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


