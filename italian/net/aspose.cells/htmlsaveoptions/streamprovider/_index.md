---
title: "HtmlSaveOptions.StreamProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Ottiene o imposta l'IStreamProvider per l'esportazione degli oggetti"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/streamprovider/
---
## HtmlSaveOptions.StreamProvider property

Ottiene o imposta l'IStreamProvider per l'esportazione degli oggetti.

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
    public class HtmlSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Crea una directory temporanea per l'output
            string outputDir = Path.Combine(Path.GetTempPath(), "AsposeStreamProviderDemo");
            Directory.CreateDirectory(outputDir);

            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("StreamProvider Demo");

            // Configura le opzioni di salvataggio HTML con un provider di stream personalizzato
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.StreamProvider = new ExportStreamProvider(outputDir);

            // Salva la cartella di lavoro come HTML
            string outputPath = Path.Combine(outputDir, "output.html");
            workbook.Save(outputPath, options);

            Console.WriteLine($"File saved with StreamProvider to: {outputPath}");
        }
    }

    public class ExportStreamProvider : IStreamProvider
    {
        private readonly string _outputDirectory;

        public ExportStreamProvider(string outputDirectory)
        {
            _outputDirectory = outputDirectory;
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Inizializzazione se necessaria
        }

        public Stream GetStream(StreamProviderOptions options)
        {
            string filePath = Path.Combine(_outputDirectory, options.CustomPath);
            return new FileStream(filePath, FileMode.Create);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Implementazione come richiesto dall'interfaccia
        }
    }
}
```

### Vedi anche

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


