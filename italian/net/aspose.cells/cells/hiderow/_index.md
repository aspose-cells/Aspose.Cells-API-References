---
title: "Cells.HideRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Nasconde una riga"
type: docs
url: /it/net/aspose.cells/cells/hiderow/
---
## Cells.HideRow method

Nasconde una riga.

```csharp
public void HideRow(int row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Nascondi la riga 5
            worksheet.Cells.HideRow(5);
            
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


