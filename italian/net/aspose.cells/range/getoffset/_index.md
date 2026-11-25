---
title: "Range.GetOffset"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Restituisce l'intervallo Range per offset"
type: docs
url: /it/net/aspose.cells/range/getoffset/
---
## Range.GetOffset method

Restituisce l'intervallo [`Range`](../) per offset.

```csharp
public Range GetOffset(int rowOffset, int columnOffset)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | Int32 | Offset di riga in questo intervallo, basato su zero. |
| columnOffset | Int32 | Offset di colonna in questo intervallo, basato su zero. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetOffsetWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Crea l'intervallo iniziale
            Aspose.Cells.Range originalRange = cells.CreateRange("A1");
            Console.WriteLine("Original Range Address: " + originalRange.Address);
            
            // Ottieni l'intervallo offset
            Aspose.Cells.Range offsetRange = originalRange.GetOffset(1, 1);
            Console.WriteLine("Offset Range Address: " + offsetRange.Address);
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


