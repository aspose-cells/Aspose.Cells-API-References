---
title: "WorksheetCollection.GetNamedRanges"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorksheetCollection. Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo"
type: docs
url: /it/net/aspose.cells/worksheetcollection/getnamedranges/
---
## WorksheetCollection.GetNamedRanges method

Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo.

```csharp
public Range[] GetNamedRanges()
```

### Valore di ritorno

Un array di oggetti Range. Se il riferimento del Nome definito è esterno o ha più intervalli, non verrà restituito alcun oggetto Range per questo Nome.

Restituisce null se l'intervallo denominato non esiste.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetNamedRangesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea alcuni intervalli denominati per dimostrazione
            worksheet.Cells.CreateRange("A1:B2").Name = "SalesData";
            worksheet.Cells.CreateRange("C3:D4").Name = "Expenses";

            try
            {
                // Chiama il metodo GetNamedRanges per recuperare tutti gli intervalli denominati
                Aspose.Cells.Range[] namedRanges = workbook.Worksheets.GetNamedRanges();

                // Visualizza le informazioni sugli intervalli denominati
                Console.WriteLine("Found {0} named ranges:", namedRanges.Length);
                foreach (Aspose.Cells.Range range in namedRanges)
                {
                    Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
                }

                // Salva la cartella di lavoro
                workbook.Save("GetNamedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNamedRanges: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


