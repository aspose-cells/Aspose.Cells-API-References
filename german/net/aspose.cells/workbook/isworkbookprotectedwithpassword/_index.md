---
title: "Workbook.IsWorkbookProtectedWithPassword"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook‑Eigenschaft. Gibt an, ob Struktur oder Fenster mit einem Passwort geschützt ist."
type: docs
url: /de/net/aspose.cells/workbook/isworkbookprotectedwithpassword/
---
## Workbook.IsWorkbookProtectedWithPassword property

Gibt an, ob Struktur oder Fenster mit einem Kennwort geschützt ist.

```csharp
public bool IsWorkbookProtectedWithPassword { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsWorkbookProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Workbook-Instanz
            Workbook workbook = new Workbook();

            // Überprüfen Sie, ob die Arbeitsmappe mit einem Passwort geschützt ist (sollte für eine neue Arbeitsmappe false sein).
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Die Arbeitsmappe mit einem Passwort schützen
            workbook.Protect(ProtectionType.All, "password123");

            // Jetzt erneut prüfen (sollte true sein).
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Arbeitsmappe entsperren.
            workbook.Unprotect("password123");

            // Endgültige Prüfung (sollte wieder false sein)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Arbeitsmappe freigeben
            workbook.Dispose();
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


