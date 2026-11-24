---
title: "Klasse SpreadsheetLocker"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.SpreadsheetLocker Klasse. Low‑Code‑API zum Sperren von Tabellendateien"
type: docs
url: /de/net/aspose.cells.lowcode/spreadsheetlocker/
---
## SpreadsheetLocker class

Low‑Code‑API zum Sperren von Tabellenkalkulationsdateien.

```csharp
public class SpreadsheetLocker
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) | Sperrt die Tabellendatei mit den angegebenen Einstellungen. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_1)(LowCodeLoadOptions, LowCodeSaveOptions, string, string) | Sperrt die Tabellendatei mit den angegebenen Einstellungen. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_3)(string, string, string, string) | Sperrt die Tabellendatei mit den angegebenen Einstellungen. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_2)(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) | Sperrt die Tabellendatei mit den angegebenen Einstellungen. |

### Beispiele

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
            // SpreadsheetLocker verwenden, um die Arbeitsmappe zu schützen
            SpreadsheetLocker.Process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


