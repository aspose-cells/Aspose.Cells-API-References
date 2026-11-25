---
title: "FindOptions.RegexKey"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FindOptions. Indica se la chiave di ricerca è una regex. Se true la chiave di ricerca verrà considerata come regex e analizzata. Altrimenti la chiave verrà analizzata secondo le regole di MS Excel"
type: docs
url: /it/net/aspose.cells/findoptions/regexkey/
---
## FindOptions.RegexKey property

Indica se la chiave cercata è una regex. Se vero, la chiave cercata verrà considerata come regex e analizzata. Altrimenti la chiave verrà analizzata secondo le regole di MS Excel.

```csharp
public bool RegexKey { get; set; }
```

### Osservazioni

Anche se la chiave di ricerca è stata specificata come regex, può essere riformulata in base al [`LookAtType`](../lookattype/) specificato. Ad esempio, quando il tipo è Contains (questo è il valore predefinito per queste opzioni), i caratteri jolly verranno aggiunti all'inizio e alla fine della chiave di ricerca automaticamente per garantire che la corrispondenza sia verificata come "contains". In questo caso, le espressioni regolari diventeranno più complesse e le prestazioni diminuiranno. Pertanto, per motivi di prestazioni, se l'utente ha specificato la regola esatta per la regex, non è necessario utilizzare [`LookAtType`](../lookattype/) come vincolo aggiuntivo e l'utente può impostarlo su EntireContent per ottenere migliori prestazioni.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta dati di test con stringhe di corrispondenza di modello
            worksheet.Cells["A1"].PutValue("[hello]");
            worksheet.Cells["A2"].PutValue("Regular text");
            worksheet.Cells["A3"].PutValue("[another_example]");

            // Crea opzioni di ricerca con regex abilitata
            FindOptions options = new FindOptions();
            options.RegexKey = true;
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;

            // Cerca le celle che corrispondono al modello regex
            string regEx = "\\[[a-zA-Z0-9_]+\\]";
            Cell foundCell = worksheet.Cells.Find(regEx, null, options);

            // Restituisci il risultato
            if (foundCell != null)
            {
                Console.WriteLine("Found cell: " + foundCell.Name + " with value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("No matching cells found");
            }
        }
    }
}
```

### Vedi anche

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


