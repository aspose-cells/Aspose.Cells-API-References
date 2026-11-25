---
title: "Cells.SetColumnWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Imposta la larghezza della colonna specificata nella visualizzazione normale"
type: docs
url: /it/net/aspose.cells/cells/setcolumnwidth/
---
## Cells.SetColumnWidth method

Imposta la larghezza della colonna specificata nella visualizzazione normale.

```csharp
public void SetColumnWidth(int column, double width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna. |
| larghezza | Double | Larghezza della colonna in unità di caratteri. La larghezza della colonna deve essere compresa tra 0 e 255. |

### Osservazioni

Per i fogli di calcolo, la larghezza della colonna è misurata come il numero di caratteri della larghezza massima delle cifre dei numeri 0~9 così come visualizzate nel carattere dello stile normale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.SetColumnWidth(0, 25.5);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


