---
title: "Workbook.Unprotect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Låser upp en arbetsbok"
type: docs
url: /sv/net/aspose.cells/workbook/unprotect/
---
## Workbook.Unprotect method

Avskyddar en arbetsbok.

```csharp
public void Unprotect(string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | String | Lösenord för att låsa upp arbetsboken. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med skydd
            Workbook workbook = new Workbook();
            workbook.Protect(ProtectionType.All, "book");

            // Lås upp arbetsboken med korrekt lösenord
            workbook.Unprotect("book");

            // Spara den oskyddade arbetsboken
            workbook.Save("unprotected_workbook.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


