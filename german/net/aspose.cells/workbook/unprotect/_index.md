---
title: "Workbook.Unprotect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Hebt den Schutz eines Arbeitsbuchs auf"
type: docs
url: /de/net/aspose.cells/workbook/unprotect/
---
## Workbook.Unprotect method

Entfernt den Schutz einer Arbeitsmappe.

```csharp
public void Unprotect(string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Passwort | String | Passwort, um den Schutz des Arbeitsbuchs aufzuheben. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Ein Arbeitsbuch mit Schutz erstellen
            Workbook workbook = new Workbook();
            workbook.Protect(ProtectionType.All, "book");

            // Das Arbeitsbuch mit dem richtigen Passwort entsperren
            workbook.Unprotect("book");

            // Das ungeschützte Arbeitsbuch speichern
            workbook.Save("unprotected_workbook.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


