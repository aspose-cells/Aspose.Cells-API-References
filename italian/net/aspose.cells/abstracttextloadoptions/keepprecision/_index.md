---
title: "AbstractTextLoadOptions.KeepPrecision"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractTextLoadOptions. Indica se non analizzare una stringa se la lunghezza è 15"
type: docs
url: /it/net/aspose.cells/abstracttextloadoptions/keepprecision/
---
## AbstractTextLoadOptions.KeepPrecision property

Indica se non analizzare un valore stringa se la lunghezza è 15.

```csharp
public bool KeepPrecision { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyKeepPrecisionDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento HTML e imposta KeepPrecision su true
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.KeepPrecision = true;

            // Carica la cartella di lavoro con le opzioni
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Dimostra che la precisione è mantenuta (ad esempio, valori numerici con molte cifre decimali)
            Cell cell = worksheet.Cells["A1"];
            Console.WriteLine("Value with precision: " + cell.Value);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


