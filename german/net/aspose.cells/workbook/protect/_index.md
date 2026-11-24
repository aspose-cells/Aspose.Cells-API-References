---
title: "Workbook.Protect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Schützt ein Workbook"
type: docs
url: /de/net/aspose.cells/workbook/protect/
---
## Workbook.Protect method

Schützt eine Arbeitsmappe.

```csharp
public void Protect(ProtectionType protectionType, string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| protectionType | ProtectionType | Schutztyp. |
| Passwort | String | Passwort zum Schützen des Workbooks. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectWithProtectionTypeStringDemo
    {
        public static void Run()
        {
            Workbook wbk = new Workbook();
            wbk.Protect(ProtectionType.Structure, "password123");
            
            wbk.Save("protected_workbook.xlsx", SaveFormat.Xlsx);
            wbk.Dispose();
        }
    }
}
```

### Siehe auch

* enum [ProtectionType](../../protectiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


