---
title: "Range.GetCellOrNull"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Ottiene l'oggetto Cell o null in questo intervallo"
type: docs
url: /it/net/aspose.cells/range/getcellornull/
---
## Range.GetCellOrNull method

Ottiene l'oggetto [`Cell`](../../cell/) o null in questo intervallo.

```csharp
public Cell GetCellOrNull(int rowOffset, int columnOffset)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | Int32 | Offset di riga in questo intervallo, basato su zero. |
| columnOffset | Int32 | Offset di colonna in questo intervallo, basato su zero. |

### Valore di ritorno

[`Cell`](../../cell/) object.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetCellOrNullWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            
            // Inserisci alcuni dati nell'intervallo
            range[0, 0].PutValue("Cell A1");
            range[0, 1].PutValue("Cell B1");
            range[1, 0].PutValue("Cell A2");
            
            // Dimostra GetCellOrNull con parametri Int32
            Cell cell1 = range.GetCellOrNull(0, 0);
            Console.WriteLine("Cell (0,0): " + (cell1 != null ? cell1.StringValue : "null"));
            
            Cell cell2 = range.GetCellOrNull(1, 1);
            Console.WriteLine("Cell (1,1): " + (cell2 != null ? cell2.StringValue : "null"));
            
            // Prova a ottenere una cella fuori dall'intervallo (dovrebbe restituire null)
            Cell cell3 = range.GetCellOrNull(2, 0);
            Console.WriteLine("Cell (2,0): " + (cell3 != null ? cell3.StringValue : "null"));
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


