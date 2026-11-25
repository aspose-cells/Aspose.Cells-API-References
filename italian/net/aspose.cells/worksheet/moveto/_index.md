---
title: "Worksheet.MoveTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Sposta il foglio in un'altra posizione nel foglio di calcolo"
type: docs
url: /it/net/aspose.cells/worksheet/moveto/
---
## Worksheet.MoveTo method

Sposta il foglio in un'altra posizione nel foglio di calcolo.

```csharp
public void MoveTo(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | Indice del foglio di destinazione. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodMoveToWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni fogli di lavoro
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Aggiungi un nuovo foglio di lavoro e spostalo nella posizione 1
            Worksheet newWorksheet = workbook.Worksheets.Add("MovedSheet");
            newWorksheet.MoveTo(1);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


