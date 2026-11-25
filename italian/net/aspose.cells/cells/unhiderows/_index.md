---
title: "Cells.UnhideRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Rende visibili le righe nascoste"
type: docs
url: /it/net/aspose.cells/cells/unhiderows/
---
## Cells.UnhideRows method

Rende visibili le righe nascoste.

```csharp
public void UnhideRows(int row, int totalRows, double height)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| totalRows | Int32 | Il numero della riga. |
| altezza | Double | Altezza della riga. L'altezza della riga verrà modificata solo quando la riga è nascosta e il valore di altezza fornito è positivo. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Nascondi le righe 0-4
            cells.HideRows(0, 5);
            
            // Rendi visibili le righe 0-4 con regolazione dell'altezza (-1 per adattamento automatico)
            cells.UnhideRows(0, 5, -1);
            
            // Verifica che le righe siano visibili
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Row {i} hidden status: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


