---
title: "Cells.HideColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Nascondi più colonne"
type: docs
url: /it/net/aspose.cells/cells/hidecolumns/
---
## Cells.HideColumns method

Nascondi più colonne.

```csharp
public void HideColumns(int column, int totalColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna. |
| totalColumns | Int32 | Numero della colonna. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola alcuni dati di esempio
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Nascondi le colonne da 3 a 5 (indice basato su zero)
            int startColumn = 2; // Column C
            int columnCount = 3;  // Hide 3 columns
            cells.HideColumns(startColumn, columnCount);

            // Salva la cartella di lavoro
            workbook.Save("HideColumnsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


