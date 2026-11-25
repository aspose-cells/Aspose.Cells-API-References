---
title: "TxtLoadOptions.HasTextQualifier"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtLoadOptions. Indica se esiste un qualificatore di testo per il valore della cella. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/txtloadoptions/hastextqualifier/
---
## TxtLoadOptions.HasTextQualifier property

Indica se è presente un qualificatore di testo per il valore della cella. Il valore predefinito è true.

```csharp
public bool HasTextQualifier { get; set; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasTextQualifierDemo
    {
        public static void Run()
        {
            // Crea contenuto CSV con qualificatori di testo
            string csvContent = "\"Name\",\"Age\",\"City\"\n\"John\",30,\"New York\"\n\"Alice\",25,\"London\"";
            
            // Salva il contenuto CSV in un file temporaneo
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvContent, Encoding.UTF8);

            // Crea TxtLoadOptions con HasTextQualifier impostato a true
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Carica il file CSV con i qualificatori di testo
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Salva la cartella di lavoro per dimostrare il caricamento riuscito
            workbook.Save("Output.xlsx");

            // Rimuovi il file temporaneo
            System.IO.File.Delete(tempFile);
        }
    }
}
```

### Vedi anche

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


