---
title: "Klass SpreadsheetLocker"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.SpreadsheetLocker-klass. Lågkods-API för att låsa kalkylbladsfil"
type: docs
url: /sv/net/aspose.cells.lowcode/spreadsheetlocker/
---
## SpreadsheetLocker class

Low-code-api för att låsa kalkylbladsfil.

```csharp
public class SpreadsheetLocker
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) | Låser kalkylbladsfilen med angivna inställningar. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_1)(LowCodeLoadOptions, LowCodeSaveOptions, string, string) | Låser kalkylbladsfilen med angivna inställningar. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_3)(string, string, string, string) | Låser kalkylbladsfilen med angivna inställningar. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_2)(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) | Låser kalkylbladsfilen med angivna inställningar. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassSpreadsheetLockerDemo
    {
        public static void Run()
        {
            // Använd SpreadsheetLocker för att skydda arbetsboken
            SpreadsheetLocker.Process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


