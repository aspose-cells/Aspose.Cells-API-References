---
title: "Range.ClearHyperlinks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Rimuove solo i collegamenti ipertestuali"
type: docs
url: /it/net/aspose.cells/range/clearhyperlinks/
---
## Range.ClearHyperlinks method

Rimuove solo i collegamenti ipertestuali.

```csharp
public void ClearHyperlinks(bool clearFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| clearFormat | Booleano | Indica se cancellare il formato dei collegamenti ipertestuali. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearHyperlinksWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo e aggiungi alcuni collegamenti ipertestuali per dimostrazione
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");
            range.AddHyperlink("https://www.example.com", "Example", "Visit Example");

            try
            {
                // Cancella i collegamenti ipertestuali con conservazione del formato (false)
                range.ClearHyperlinks(false);
                Console.WriteLine("Hyperlinks cleared while preserving format");

                // Aggiungi nuovamente i collegamenti ipertestuali
                range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");

                // Cancella i collegamenti ipertestuali senza conservazione del formato (true)
                range.ClearHyperlinks(true);
                Console.WriteLine("Hyperlinks cleared without preserving format");

                // Salva la cartella di lavoro
                workbook.Save("ClearHyperlinksDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


