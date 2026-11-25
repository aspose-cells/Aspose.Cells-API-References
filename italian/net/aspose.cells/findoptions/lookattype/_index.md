---
title: "FindOptions.LookAtType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FindOptions. Tipo di ricerca"
type: docs
url: /it/net/aspose.cells/findoptions/lookattype/
---
## FindOptions.LookAtType property

Guarda il tipo.

```csharp
public LookAtType LookAtType { get; set; }
```

### Osservazioni

Quando [`RegexKey`](../regexkey/) è true e l'utente ha specificato la regola esatta per la regex, per motivi di prestazioni questa proprietà dovrebbe essere impostata su EntireContent. Altrimenti ristruttureremo la chiave di ricerca per garantire che possa essere corrispondente al tipo specifico. Ad esempio, quando il tipo è Contains (questo è il valore predefinito per questa proprietà), aggiungeremo automaticamente i caratteri jolly all'inizio e alla fine della chiave di ricerca. In questo caso, le espressioni regolari diventeranno più complesse e le prestazioni diminuiranno.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookAtTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e aggiungi alcuni dati
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("=1+2"); // Formula
            worksheet.Cells["A3"].PutValue("Partial match test");
            worksheet.Cells["A4"].PutValue("=A1&A3"); // Formula concatenating cells

            // Crea le opzioni di ricerca con LookAtType.EntireContent
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.EntireContent
            };

            // Cerca la formula che corrisponde esattamente a "=A1&A3"
            Cell cell = worksheet.Cells.Find("=A1&A3", null, options);
            Console.WriteLine("Found cell with exact formula match: " + (cell != null ? cell.Name : "null"));

            // Passa a corrispondenza parziale
            options.LookAtType = LookAtType.Contains;
            cell = worksheet.Cells.Find("A3", null, options);
            Console.WriteLine("Found cell containing 'A3' in formula: " + (cell != null ? cell.Name : "null"));
        }
    }
}
```

### Vedi anche

* enum [LookAtType](../../lookattype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


