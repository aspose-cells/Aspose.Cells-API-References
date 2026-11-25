---
title: "Cells.SetRowHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Imposta l'altezza della riga specificata"
type: docs
url: /it/net/aspose.cells/cells/setrowheight/
---
## Cells.SetRowHeight method

Imposta l'altezza della riga specificata.

```csharp
public void SetRowHeight(int row, double height)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga. |
| altezza | Double | Altezza della riga. In unità di punto, deve essere compresa tra 0 e 409,5. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta l'altezza della riga per la prima riga (indice 0) a 25,5 punti
            cells.SetRowHeight(0, 25.5);

            // Verifica l'altezza della riga
            Console.WriteLine("Row height of row 0: " + cells.GetRowHeight(0));
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


