---
title: "Range.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Ottiene e imposta il valore dell'intervallo"
type: docs
url: /it/net/aspose.cells/range/value/
---
## Range.Value property

Ottiene e imposta il valore dell'intervallo.

```csharp
public object Value { get; set; }
```

### Osservazioni

Se l'intervallo contiene più celle, l'oggetto restituito/applicato dovrebbe essere un oggetto Array bidimensionale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo a partire da A1 che copre 3x3 celle
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");

            // Imposta un array 2D come valore per l'intervallo
            int[,] values = new int[3, 3] { { 1, 2, 3 }, { 4, 5, 6 }, { 7, 8, 9 } };
            range.Value = values;

            // Salva la cartella di lavoro
            workbook.Save("RangePropertyValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


