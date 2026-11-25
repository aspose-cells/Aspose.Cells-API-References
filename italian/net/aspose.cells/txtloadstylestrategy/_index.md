---
title: "Enum TxtLoadStyleStrategy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.TxtLoadStyleStrategy. Specifica come applicare lo stile ai valori analizzati quando si converte una stringa in numero o data/ora"
type: docs
url: /it/net/aspose.cells/txtloadstylestrategy/
---
## TxtLoadStyleStrategy enumeration

Specifica come applicare lo stile ai valori analizzati quando si converte una stringa in numero o data/ora.

```csharp
public enum TxtLoadStyleStrategy
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Non imposta lo stile per il valore analizzato. |
| BuiltIn | `1` | Imposta lo stile come numero/data‑ora predefinito quando il valore analizzato è un semplice valore numerico/data‑ora. |
| ExactFormat | `2` | Imposta il formato personalizzato esatto per il valore analizzato in modo che il valore formattato sia identico all'input originale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtLoadStyleStrategyDemo
    {
        public static void TxtLoadStyleStrategyExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definisci un contenuto CSV di esempio
            string csvContent = "Name,Date,Value\nJohn,2023-01-01,100\nDoe,2023-01-02,200";

            // Salva il contenuto CSV in un file temporaneo
            string tempCsvFilePath = "sample.csv";
            System.IO.File.WriteAllText(tempCsvFilePath, csvContent);

            // Crea TxtLoadOptions e imposta LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.ExactFormat;

            // Carica il file CSV nella cartella di lavoro
            workbook = new Workbook(tempCsvFilePath, loadOptions);

            // Salva la cartella di lavoro in un file Excel
            workbook.Save("TxtLoadStyleStrategyExample.xlsx");

            // Pulisci il file CSV temporaneo
            System.IO.File.Delete(tempCsvFilePath);

            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


