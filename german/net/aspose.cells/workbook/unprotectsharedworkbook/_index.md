---
title: "Workbook.UnprotectSharedWorkbook"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Hebt den Schutz eines freigegebenen Workbooks auf"
type: docs
url: /de/net/aspose.cells/workbook/unprotectsharedworkbook/
---
## Workbook.UnprotectSharedWorkbook method

Entfernt den Schutz einer freigegebenen Arbeitsmappe.

```csharp
public void UnprotectSharedWorkbook(string password)
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
    public class WorkbookMethodUnprotectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Schützen Sie die gemeinsam genutzte Arbeitsmappe mit einem Passwort
            wb.ProtectSharedWorkbook("abcd");
            
            // Speichern Sie die geschützte Arbeitsmappe
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Arbeitsmappe erneut öffnen
            wb = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Entferne den Schutz des freigegebenen Workbooks mit Passwort
            wb.UnprotectSharedWorkbook("abcd");
            
            // Das ungeschützte Arbeitsbuch speichern
            wb.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


