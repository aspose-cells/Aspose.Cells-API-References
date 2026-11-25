---
title: "Interfaccia IFilePathProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Interfaccia Aspose.Cells.IFilePathProvider. Rappresenta il provider del percorso file esportato"
type: docs
url: /it/net/aspose.cells/ifilepathprovider/
---
## IFilePathProvider interface

Rappresenta il provider del percorso del file esportato.

```csharp
public interface IFilePathProvider
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetFullName](../../aspose.cells/ifilepathprovider/getfullname/)(string) | Ottiene il percorso completo del file in base al nome del foglio di lavoro quando si esporta il foglio di lavoro in HTML separatamente. In questo modo i riferimenti tra i fogli di lavoro possono essere esportati correttamente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderDemo : IFilePathProvider
    {
        // Implementazione del metodo GetFullName dell'interfaccia IFilePathProvider
        public string GetFullName(string sheetName)
        {
            // Per dimostrazione, restituisce un percorso file semplice basato sul nome del foglio
            return $"{sheetName}.html";
        }

        public static void IFilePathProviderExample()
        {
            // Crea una nuova cartella di lavoro e aggiungi alcuni dati
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Crea HtmlSaveOptions e imposta il FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new IFilePathProviderDemo();

            // Salva la cartella di lavoro in formato HTML
            workbook.Save("IFilePathProviderExample.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }


}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


