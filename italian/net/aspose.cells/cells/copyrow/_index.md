---
title: "Cells.CopyRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Copia i dati e i formati di un'intera riga"
type: docs
url: /it/net/aspose.cells/cells/copyrow/
---
## Cells.CopyRow method

Copia i dati e i formati di un'intera riga.

```csharp
public void CopyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | Celle | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceRowIndex | Int32 | Indice della riga di origine. |
| destinationRowIndex | Int32 | Indice della riga di destinazione. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet1 = workbook.Worksheets[0];
            Cells cells1 = worksheet1.Cells;
            
            // Aggiungi alcuni dati alla prima riga
            cells1["A1"].PutValue("Source Data");
            cells1["B1"].PutValue(100);
            cells1["C1"].PutValue(DateTime.Now);
            
            // Crea il secondo foglio di lavoro
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            Cells cells2 = worksheet2.Cells;
            
            // Copia la riga da Sheet1 a Sheet2
            cells2.CopyRow(cells1, 0, 0);
            
            // Copia la riga all'interno di Sheet1 in nuove posizioni
            cells1.CopyRow(cells1, 0, 1);
            cells1.CopyRow(cells1, 0, 2);
            
            // Salva la cartella di lavoro
            workbook.Save("CopyRowExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


