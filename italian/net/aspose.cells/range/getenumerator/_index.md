---
title: "Range.GetEnumerator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Ottiene l'enumeratore per le celle in questo Range"
type: docs
url: /it/net/aspose.cells/range/getenumerator/
---
## Range.GetEnumerator method

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
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola alcuni dati di esempio
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["C2"].PutValue("Cherry");
            worksheet.Cells["C3"].PutValue("Date");

            // Ottieni l'intervallo e enumera le celle
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C3");
            IEnumerator enumerator = range.GetEnumerator();
            
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine($"{cell.Name}: {cell.Value}");
            }
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


