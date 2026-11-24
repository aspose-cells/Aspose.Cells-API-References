---
title: "Workbook.ProtectSharedWorkbook"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Schützt eine freigegebene Arbeitsmappe"
type: docs
url: /de/net/aspose.cells/workbook/protectsharedworkbook/
---
## Workbook.ProtectSharedWorkbook method

Schützt eine freigegebene Arbeitsmappe.

```csharp
public void ProtectSharedWorkbook(string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Passwort | String | Passwort zum Schützen des Workbooks. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Schützen Sie die gemeinsam genutzte Arbeitsmappe mit einem Passwort
            wb.ProtectSharedWorkbook("abcd");
            
            // Speichern Sie die geschützte Arbeitsmappe
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Laden Sie die geschützte Arbeitsmappe
            Workbook wbProtected = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Überprüfen Sie den Schutzstatus
            Console.WriteLine("Workbook is protected: " + wbProtected.Settings.IsProtected);
            
            // Arbeitsmappe entsperren.
            wbProtected.UnprotectSharedWorkbook("abcd");
            
            // Das ungeschützte Arbeitsbuch speichern
            wbProtected.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


