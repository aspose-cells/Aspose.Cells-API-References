---
title: "Workbook.Protect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook method. Skyddar en workbook"
type: docs
url: /sv/net/aspose.cells/workbook/protect/
---
## Workbook.Protect method

Skyddar en arbetsbok.

```csharp
public void Protect(ProtectionType protectionType, string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| protectionType | ProtectionType | Skyddstyp. |
| lösenord | String | Lösenord för att skydda workbooken. |

### Exempel

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

### Se även

* enum [ProtectionType](../../protectiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


