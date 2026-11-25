---
title: "Range.CopyData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Copia i dati delle celle, incluse le formule, da un intervallo di origine"
type: docs
url: /it/net/aspose.cells/range/copydata/
---
## Range.CopyData method

Copia i dati della cella (incluse le formule) da un intervallo di origine.

```csharp
public void CopyData(Range range)
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
    public class RangeMethodCopyDataWithRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni il primo foglio di lavoro e aggiungi alcuni dati
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            sheetSrc.Cells["A1"].PutValue("Source Data");
            sheetSrc.Cells["B1"].PutValue(100);
            sheetSrc.Cells["A2"].PutValue("More Data");
            sheetSrc.Cells["B2"].PutValue(200);

            // Aggiungi un foglio di lavoro di destinazione
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";

            // Crea intervalli di origine e di destinazione
            Aspose.Cells.Range rangeSrc = sheetSrc.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("C3:D4");

            // Copia i dati dall'intervallo di origine all'intervallo di destinazione
            rangeDest.CopyData(rangeSrc);

            // Salva la cartella di lavoro
            workbook.Save("RangeCopyDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


