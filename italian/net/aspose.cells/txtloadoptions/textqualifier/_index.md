---
title: "TxtLoadOptions.TextQualifier"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtLoadOptions. Specifica il qualificatore di testo per i valori delle celle. Il qualificatore predefinito è"
type: docs
url: /it/net/aspose.cells/txtloadoptions/textqualifier/
---
## TxtLoadOptions.TextQualifier property

Specifica il qualificatore di testo per i valori delle celle. Il qualificatore predefinito è '\"'.

```csharp
public char TextQualifier { get; set; }
```

### Osservazioni

Quando si imposta questa proprietà, [`HasTextQualifier`](../hastextqualifier/) diventerà true automaticamente.

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTextQualifierDemo
    {
        public static void Run()
        {
            // Crea un'istanza di TxtLoadOptions per CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Crea dati CSV di esempio con qualificatori di testo
            string csvData = "Name,Age,City\n\"John Doe\",30,\"New York\"\n\"Jane Smith\",25,\"San Francisco\"";
            
            // Salva i dati di esempio in un file temporaneo
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvData);

            // Carica il file CSV con le opzioni specificate
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Salva la cartella di lavoro in un file Excel
            workbook.Save("TextQualifierDemo.xlsx");

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


