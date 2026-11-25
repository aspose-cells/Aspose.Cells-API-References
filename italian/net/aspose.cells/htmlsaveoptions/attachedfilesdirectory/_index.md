---
title: "HtmlSaveOptions.AttachedFilesDirectory"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. La directory in cui verranno salvati i file allegati. Solo per il salvataggio in uno stream HTML."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/attachedfilesdirectory/
---
## HtmlSaveOptions.AttachedFilesDirectory property

La directory in cui verranno salvati i file allegati. Solo per il salvataggio in stream html.

```csharp
public string AttachedFilesDirectory { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // Crea una directory temporanea per la dimostrazione.
            string tempDir = Path.Combine(Path.GetTempPath(), "AsposeAttachedFilesDemo");
            Directory.CreateDirectory(tempDir);

            try
            {
                // Crea una cartella di lavoro di esempio
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Hello World");

                // Imposta le opzioni di salvataggio HTML con AttachedFilesDirectory.
                HtmlSaveOptions options = new HtmlSaveOptions();
                options.AttachedFilesDirectory = tempDir;

                // Salva la cartella di lavoro come HTML
                string outputPath = Path.Combine(tempDir, "output.html");
                workbook.Save(outputPath, options);

                // Verifica che i file allegati siano stati creati.
                Console.WriteLine("HTML saved with attached files in: " + tempDir);
                Console.WriteLine("Attached files exist: " + 
                    File.Exists(Path.Combine(tempDir, "sheet001.htm")));
            }
            finally
            {
                // Pulisci
                Directory.Delete(tempDir, true);
            }
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


