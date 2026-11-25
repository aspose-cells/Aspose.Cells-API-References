---
title: "SaveOptions.CachedFileFolder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SaveOptions. La cartella per i file temporanei che possono essere usati come cache dei dati"
type: docs
url: /it/net/aspose.cells/saveoptions/cachedfilefolder/
---
## SaveOptions.CachedFileFolder property

La cartella per i file temporanei che possono essere usati come cache dei dati.

```csharp
public string CachedFileFolder { get; set; }
```

### Osservazioni

Se la cartella non è stata specificata, il valore predefinito è [`GetCacheFolder`](../../cellshelper/getcachefolder/). Se il suo valore predefinito è null o vuoto, o è stato specificato come null o vuoto, allora non verrà utilizzato alcun file di cache durante il salvataggio della cartella di lavoro.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCachedFileFolderDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test cached file folder");

            // Imposta le opzioni di salvataggio con la cartella dei file nella cache
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.CachedFileFolder = "TempCache"; // Specify cache folder

            // Salva la cartella di lavoro
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with cached file folder option.");
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


