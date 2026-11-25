---
title: "Cells.HideGroupDetail"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Comprimi le righe/colonne raggruppate"
type: docs
url: /it/net/aspose.cells/cells/hidegroupdetail/
---
## Cells.HideGroupDetail method

Comprimi le righe/colonne raggruppate.

```csharp
public void HideGroupDetail(bool isVertical, int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isVertical | Booleano | True, comprimi le righe raggruppate. |
| indice | Int32 | L'indice di riga/colonna |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Raggruppa le righe e nascondi i dettagli
            worksheet.Cells.GroupRows(0, 9, false);
            worksheet.Cells.HideGroupDetail(true, 4);
            worksheet.Cells.HideGroupDetail(true, 7);

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


