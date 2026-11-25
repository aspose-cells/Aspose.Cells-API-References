---
title: "Range.CopyValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Copia il valore della cella da un intervallo di origine"
type: docs
url: /it/net/aspose.cells/range/copyvalue/
---
## Range.CopyValue method

Copia il valore della cella da un intervallo di origine.

```csharp
public void CopyValue(Range range)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | Range | Oggetto [`Range`](../) di origine. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyValueWithRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e ottieni il primo foglio di lavoro
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "SourceSheet";
            
            // Aggiungi un altro foglio di lavoro per la destinazione
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "DestinationSheet";
            
            // Crea dati di esempio nell'intervallo di origine
            Cells cellsSrc = sheetSrc.Cells;
            cellsSrc["A1"].PutValue("Source Data");
            cellsSrc["A2"].PutValue(10);
            cellsSrc["B2"].PutValue(20);
            cellsSrc["A3"].PutValue(30);
            cellsSrc["B3"].PutValue(40);
            
            // Crea intervalli per origine e destinazione
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A2:B3");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("D2:E3");
            
            // Copia i valori dall'intervallo di origine all'intervallo di destinazione
            rangeDest.CopyValue(rangeSrc);
            
            // Salva la cartella di lavoro
            workbook.Save("RangeCopyValueDemo.xlsx");
            
            Console.WriteLine("Values copied successfully from source range to destination range.");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


