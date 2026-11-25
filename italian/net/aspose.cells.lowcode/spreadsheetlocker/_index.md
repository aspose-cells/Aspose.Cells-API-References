---
title: "Classe SpreadsheetLocker"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LowCode.SpreadsheetLocker. API low‑code per bloccare il file del foglio di calcolo"
type: docs
url: /it/net/aspose.cells.lowcode/spreadsheetlocker/
---
## SpreadsheetLocker class

API low‑code per bloccare il file di foglio di calcolo.

```csharp
public class SpreadsheetLocker
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) | Blocca il file del foglio di calcolo con le impostazioni specificate. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_1)(LowCodeLoadOptions, LowCodeSaveOptions, string, string) | Blocca il file del foglio di calcolo con le impostazioni specificate. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_3)(string, string, string, string) | Blocca il file del foglio di calcolo con le impostazioni specificate. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_2)(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) | Blocca il file del foglio di calcolo con le impostazioni specificate. |

### Esempi

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
            // Usa SpreadsheetLocker per proteggere la cartella di lavoro
            SpreadsheetLocker.Process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


