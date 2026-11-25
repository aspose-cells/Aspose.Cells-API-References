---
title: "Cells.HideColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Nasconde una colonna"
type: docs
url: /it/net/aspose.cells/cells/hidecolumn/
---
## Cells.HideColumn method

Nasconde una colonna.

```csharp
public void HideColumn(int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta alcuni dati nella colonna che nasconderemo
            cells["B1"].PutValue("This column will be hidden");
            cells["B2"].PutValue(123.45);

            // Nascondi la colonna B (indice 1)
            cells.HideColumn(1);

            // Rendi visibile la colonna con larghezza standard
            cells.UnhideColumn(1, cells.StandardWidth);

            // Salva la cartella di lavoro
            workbook.Save("HideColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


