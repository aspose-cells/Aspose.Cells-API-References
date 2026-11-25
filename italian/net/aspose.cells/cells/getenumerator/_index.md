---
title: "Cells.GetEnumerator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'enumeratore delle celle"
type: docs
url: /it/net/aspose.cells/cells/getenumerator/
---
## Cells.GetEnumerator method

Restituisce l'enumeratore delle celle.

```csharp
public IEnumerator GetEnumerator()
```

### Valore di ritorno

L'enumeratore delle celle

### Osservazioni

Durante l'attraversamento degli elementi tramite l'Enumerator restituito, la raccolta di celle non dovrebbe essere modificata(ad esempio operazioni che provocheranno l'istanziazione di nuove Cell/Row o l'eliminazione di Cell/Row esistenti). Altrimenti l'enumerator potrebbe non riuscire ad attraversare correttamente tutte le celle(alcuni elementi potrebbero essere attraversati più volte o saltati).

### Esempi

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            
            // Ottieni l'enumeratore e itera attraverso le celle
            IEnumerator enumerator = worksheet.Cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                if (cell.Value != null)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


