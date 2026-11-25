---
title: "Cells.InsertRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Inserisce una nuova riga nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/insertrow/
---
## Cells.InsertRow method

Inserisce una nuova riga nel foglio di lavoro.

```csharp
public void InsertRow(int rowIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Indice della riga. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ottieni la raccolta di celle
            Cells cells = sheet.Cells;
            
            // Inserisci dati di esempio nella riga 6
            cells[6, 0].PutValue("Original Row 6");
            cells[6, 1].PutValue(100);
            
            // Inserisci dati di esempio nella riga 7
            cells[7, 0].PutValue("Original Row 7");
            cells[7, 1].PutValue(200);
            
            // Inserisci una nuova riga all'indice 7 (spinge la riga 7 esistente verso il basso)
            cells.InsertRow(7);
            
            // Aggiungi dati alla riga appena inserita
            cells[7, 0].PutValue("New Inserted Row");
            cells[7, 1].PutValue(150);
            
            // Salva la cartella di lavoro
            workbook.Save("InsertRowDemo.xlsx");
            
            Console.WriteLine("Row inserted successfully at index 7.");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


