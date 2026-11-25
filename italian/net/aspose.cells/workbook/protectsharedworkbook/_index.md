---
title: "Workbook.ProtectSharedWorkbook"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Protegge una cartella di lavoro condivisa"
type: docs
url: /it/net/aspose.cells/workbook/protectsharedworkbook/
---
## Workbook.ProtectSharedWorkbook method

Protegge una cartella di lavoro condivisa.

```csharp
public void ProtectSharedWorkbook(string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | Password per proteggere il workbook. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Proteggi la cartella di lavoro condivisa con una password
            wb.ProtectSharedWorkbook("abcd");
            
            // Salva la cartella di lavoro protetta
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Carica la cartella di lavoro protetta
            Workbook wbProtected = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Verifica lo stato della protezione
            Console.WriteLine("Workbook is protected: " + wbProtected.Settings.IsProtected);
            
            // Rimuovi la protezione dalla cartella di lavoro
            wbProtected.UnprotectSharedWorkbook("abcd");
            
            // Salva il workbook non protetto
            wbProtected.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


