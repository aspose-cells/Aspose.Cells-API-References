---
title: "SaveOptions.CreateDirectory"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SaveOptions. Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file"
type: docs
url: /it/net/aspose.cells/saveoptions/createdirectory/
---
## SaveOptions.CreateDirectory property

Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.

```csharp
public bool CreateDirectory { get; set; }
```

### Osservazioni

Il valore predefinito è false.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCreateDirectoryDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Imposta le opzioni di salvataggio con CreateDirectory abilitato
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.CreateDirectory = true;

            // Salva la cartella di lavoro in una nuova directory (verrà creata automaticamente)
            string outputPath = "OutputDirectory/example.xls";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved successfully with directory creation.");
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


