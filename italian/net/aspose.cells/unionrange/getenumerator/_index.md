---
title: "UnionRange.GetEnumerator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo UnionRange. Restituisce l'enumeratore per le celle in questo intervallo"
type: docs
url: /it/net/aspose.cells/unionrange/getenumerator/
---
## UnionRange.GetEnumerator method

Ottiene l'enumeratore per le celle in questo Intervallo.

```csharp
public IEnumerator GetEnumerator()
```

### Valore di ritorno

L'enumeratore delle celle

### Osservazioni

Durante l'attraversamento degli elementi tramite l'Enumerator restituito, la raccolta di celle non dovrebbe essere modificata(ad esempio operazioni che provocheranno l'istanziazione di nuove Cell/Row o l'eliminazione di Cell/Row esistenti). Altrimenti l'enumerator potrebbe non riuscire ad attraversare correttamente tutte le celle(alcuni elementi potrebbero essere attraversati più volte o saltati).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class UnionRangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea il primo intervallo (A1:B2) e riempilo con i dati
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1", "B2");
            range1[0, 0].PutValue("R1C1");
            range1[0, 1].PutValue("R1C2");
            range1[1, 0].PutValue("R2C1");
            range1[1, 1].PutValue("R2C2");

            // Crea il secondo intervallo (C1:D2) e riempilo con i dati
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1", "D2");
            range2[0, 0].PutValue("R1C3");
            range2[0, 1].PutValue("R1C4");
            range2[1, 0].PutValue("R2C3");
            range2[1, 1].PutValue("R2C4");

            try
            {
                // Crea un UnionRange dal primo intervallo
                UnionRange unionRange = worksheet.Cells
                    .CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { range1 });

                // Aggiungi il secondo intervallo all'unione
                unionRange = unionRange.Union("C1:D2");

                // Ottieni l'enumeratore e itera attraverso tutte le celle nell'unione
                IEnumerator enumerator = unionRange.GetEnumerator();
                Console.WriteLine("Enumerating cells in the UnionRange:");
                while (enumerator.MoveNext())
                {
                    Cell cell = enumerator.Current as Cell;
                    if (cell != null)
                    {
                        Console.WriteLine($"{cell.Name}: {cell.Value}");
                    }
                }

                // Salva la cartella di lavoro (opzionale, solo per mostrare che i dati persistono)
                workbook.Save("UnionRangeGetEnumeratorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetEnumerator: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


