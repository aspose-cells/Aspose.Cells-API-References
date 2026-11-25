---
title: "Interfaccia IStreamProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Interfaccia Aspose.Cells.IStreamProvider. Rappresenta il provider di stream esportato"
type: docs
url: /it/net/aspose.cells/istreamprovider/
---
## IStreamProvider interface

Rappresenta il provider del flusso esportato.

```csharp
public interface IStreamProvider
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CloseStream](../../aspose.cells/istreamprovider/closestream/)(StreamProviderOptions) | Chiude lo stream. |
| [InitStream](../../aspose.cells/istreamprovider/initstream/)(StreamProviderOptions) | Ottiene lo stream. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IStreamProviderDemo : IStreamProvider
    {
        // Implementazione del metodo InitStream
        public void InitStream(StreamProviderOptions options)
        {
            string outputDir = "/test/";
            string path = outputDir + Path.GetFileName(options.DefaultPath);
            options.CustomPath = path;
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
        }

        // Implementazione del metodo CloseStream
        public void CloseStream(StreamProviderOptions options)
        {
            // Chiudi lo stream se non è nullo
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }

        public static void IStreamProviderExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta alcuni dati nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Hello World");

            // Crea HtmlSaveOptions e imposta lo StreamProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new IStreamProviderDemo();

            // Salva la cartella di lavoro in formato HTML
            workbook.Save("IStreamProviderExample.html", saveOptions);

            // Carica la cartella di lavoro dal formato HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new IStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("IStreamProviderExample.html", loadOptions);

            // Visualizza i dati caricati
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }

}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


