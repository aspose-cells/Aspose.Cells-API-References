---
title: "Workbook.Protect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo del workbook. Protegge un workbook"
type: docs
url: /it/net/aspose.cells/workbook/protect/
---
## Workbook.Protect method

Protegge una cartella di lavoro.

```csharp
public void Protect(ProtectionType protectionType, string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| protectionType | ProtectionType | Tipo di protezione. |
| password | String | Password per proteggere il workbook. |

### Esempi

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

### Vedi anche

* enum [ProtectionType](../../protectiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


