---
title: "Workbook.UnprotectSharedWorkbook"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Workbook method. Rimuove la protezione da una cartella di lavoro condivisa"
type: docs
url: /it/net/aspose.cells/workbook/unprotectsharedworkbook/
---
## Workbook.UnprotectSharedWorkbook method

Rimuove la protezione da una cartella di lavoro condivisa.

```csharp
public void UnprotectSharedWorkbook(string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | Password per rimuovere la protezione del workbook. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUnprotectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Proteggi la cartella di lavoro condivisa con una password
            wb.ProtectSharedWorkbook("abcd");
            
            // Salva la cartella di lavoro protetta
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Riapri la cartella di lavoro
            wb = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Rimuovi la protezione della cartella di lavoro condivisa con password
            wb.UnprotectSharedWorkbook("abcd");
            
            // Salva il workbook non protetto
            wb.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


