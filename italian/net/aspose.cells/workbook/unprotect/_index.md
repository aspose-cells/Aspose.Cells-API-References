---
title: "Workbook.Unprotect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Rimuove la protezione da un workbook"
type: docs
url: /it/net/aspose.cells/workbook/unprotect/
---
## Workbook.Unprotect method

Rimuove la protezione da una cartella di lavoro.

```csharp
public void Unprotect(string password)
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
    public class WorkbookMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Crea un workbook con protezione
            Workbook workbook = new Workbook();
            workbook.Protect(ProtectionType.All, "book");

            // Rimuovi la protezione del workbook con la password corretta
            workbook.Unprotect("book");

            // Salva il workbook non protetto
            workbook.Save("unprotected_workbook.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


