---
title: "HtmlSaveOptions.FilePathProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Ottiene o imposta l'IFilePathProvider per esportare il Worksheet in html separatamente"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/filepathprovider/
---
## HtmlSaveOptions.FilePathProvider property

Ottiene o imposta l'IFilePathProvider per l'esportazione del Worksheet in html separatamente.

```csharp
public IFilePathProvider FilePathProvider { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFilePathProviderDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e aggiungi alcuni dati
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Crea HtmlSaveOptions e imposta il FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new CustomFilePathProvider();

            // Salva la cartella di lavoro in formato HTML
            workbook.Save("output.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }

    public class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Logica personalizzata per generare percorsi file
            return $"custom_{sheetName}";
        }
    }
}
```

### Vedi anche

* interface [IFilePathProvider](../../ifilepathprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


