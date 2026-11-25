---
title: "Cells.UnhideColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Rende visibile una colonna"
type: docs
url: /it/net/aspose.cells/cells/unhidecolumn/
---
## Cells.UnhideColumn method

Rende visibile una colonna

```csharp
public void UnhideColumn(int column, double width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna. |
| larghezza | Double | Larghezza colonna. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideColumnWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Nascondi colonna 2
            cells.HideColumn(2);
            
            // Rivela colonna 2 con regolazione della larghezza (-1 indica l'uso della larghezza standard)
            cells.UnhideColumn(2, -1);
            
            Console.WriteLine("Column 2 width after unhiding: " + cells.Columns[2].Width);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


