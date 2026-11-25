---
title: "MarkdownSaveOptions.StreamProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MarkdownSaveOptions proprietà. Ottiene o imposta l'IStreamProvider per l'esportazione degli oggetti. Se null, gli oggetti esportati saranno salvati nella stessa directory del file di output"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/streamprovider/
---
## MarkdownSaveOptions.StreamProvider property

Ottiene o imposta l'IStreamProvider per l'esportazione degli oggetti. Se `null`, gli oggetti esportati saranno salvati nella stessa directory del file di output.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MarkdownSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].Value = "Hello";
            worksheet.Cells["B1"].Value = "World";

            try
            {
                // Crea un'istanza di MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Visualizza il valore corrente di StreamProvider (null per impostazione predefinita)
                Console.WriteLine("Current StreamProvider: " + (saveOptions.StreamProvider == null ? "null" : "set"));

                // Crea un'implementazione personalizzata di StreamProvider
                CustomStreamProvider streamProvider = new CustomStreamProvider();
                saveOptions.StreamProvider = streamProvider;

                // Visualizza il valore aggiornato di StreamProvider
                Console.WriteLine("Updated StreamProvider: " + (saveOptions.StreamProvider != null ? "set" : "null"));

                // Salva la cartella di lavoro con lo StreamProvider personalizzato
                workbook.Save("StreamProviderDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved with custom StreamProvider.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    // Implementazione personalizzata di IStreamProvider
    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            Console.WriteLine("Initializing stream");
        }

        public void CloseStream(StreamProviderOptions options)
        {
            Console.WriteLine("Closing stream");
        }
    }
}
```

### Vedi anche

* interface [IStreamProvider](../../istreamprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


