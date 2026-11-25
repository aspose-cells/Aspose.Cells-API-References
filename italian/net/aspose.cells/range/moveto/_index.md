---
title: "Range.MoveTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Sposta l'intervallo corrente nell'intervallo di destinazione"
type: docs
url: /it/net/aspose.cells/range/moveto/
---
## Range.MoveTo method

Sposta l'intervallo corrente nell'intervallo di destinazione.

```csharp
public void MoveTo(int destRow, int destColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destRow | Int32 | La riga iniziale dell'intervallo di destinazione. |
| destColumn | Int32 | La colonna iniziale dell'intervallo di destinazione. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo di esempio (A1:B2)
            Aspose.Cells.Range originalRange = worksheet.Cells.CreateRange("A1", "B2");
            
            // Inserisci alcuni dati nell'intervallo per dimostrazione
            originalRange[0, 0].PutValue("A1");
            originalRange[0, 1].PutValue("B1");
            originalRange[1, 0].PutValue("A2");
            originalRange[1, 1].PutValue("B2");
            
            // Sposta l'intervallo verso il basso di 1 riga (a A2:B3)
            originalRange.MoveTo(originalRange.FirstRow + 1, originalRange.FirstColumn);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


