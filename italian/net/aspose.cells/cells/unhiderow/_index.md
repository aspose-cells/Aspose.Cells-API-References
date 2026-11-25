---
title: "Cells.UnhideRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Rende visibile una riga"
type: docs
url: /it/net/aspose.cells/cells/unhiderow/
---
## Cells.UnhideRow method

Rende visibile una riga.

```csharp
public void UnhideRow(int row, double height)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga. |
| altezza | Double | Altezza della riga. L'altezza della riga verrà modificata solo quando la riga è nascosta e il valore di altezza fornito è positivo. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Nascondi la riga 5
            worksheet.Cells.HideRow(5);
            
            // Mostra la riga 5 con un'altezza di 12.75
            worksheet.Cells.UnhideRow(5, 12.75);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


