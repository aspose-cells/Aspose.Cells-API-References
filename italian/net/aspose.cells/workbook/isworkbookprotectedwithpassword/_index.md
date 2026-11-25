---
title: "Workbook.IsWorkbookProtectedWithPassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Indica se la struttura o la finestra è protetta da password"
type: docs
url: /it/net/aspose.cells/workbook/isworkbookprotectedwithpassword/
---
## Workbook.IsWorkbookProtectedWithPassword property

Indica se la struttura o la finestra è protetta da password.

```csharp
public bool IsWorkbookProtectedWithPassword { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsWorkbookProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Crea una nuova istanza di Workbook
            Workbook workbook = new Workbook();

            // Verifica se la cartella di lavoro è protetta da password (dovrebbe essere false per una nuova cartella di lavoro)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Proteggi la cartella di lavoro con una password
            workbook.Protect(ProtectionType.All, "password123");

            // Ora verifica di nuovo (dovrebbe essere true)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Rimuovi la protezione dalla cartella di lavoro
            workbook.Unprotect("password123");

            // Verifica finale (dovrebbe essere false di nuovo)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Elimina la cartella di lavoro
            workbook.Dispose();
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


