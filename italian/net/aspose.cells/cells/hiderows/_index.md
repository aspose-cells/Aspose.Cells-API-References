---
title: "Cells.HideRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Nasconde più righe"
type: docs
url: /it/net/aspose.cells/cells/hiderows/
---
## Cells.HideRows method

Nasconde più righe.

```csharp
public void HideRows(int row, int totalRows)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| totalRows | Int32 | Il numero della riga. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i+1}, Col {j+1}";
                }
            }

            // Nascondi le righe 3-5 (indice basato su zero: 2-4)
            worksheet.Cells.HideRows(2, 3);

            // Salva la cartella di lavoro
            workbook.Save("HideRowsExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


