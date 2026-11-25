---
title: "Range.IsBlank"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Indica se l'intervallo contiene valori"
type: docs
url: /it/net/aspose.cells/range/isblank/
---
## Range.IsBlank method

Indica se l'intervallo contiene valori.

```csharp
public bool IsBlank()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea un intervallo e verifica se è vuoto (dovrebbe essere vero)
            Aspose.Cells.Range range1 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank: " + range1.IsBlank());

            // Inserisci un valore in una cella e verifica di nuovo (dovrebbe essere falso)
            cells["B2"].PutValue("Test");
            Aspose.Cells.Range range2 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank after adding value: " + range2.IsBlank());
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


