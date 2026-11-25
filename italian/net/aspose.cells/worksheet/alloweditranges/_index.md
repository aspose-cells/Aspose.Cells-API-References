---
title: "Worksheet.AllowEditRanges"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Worksheet property. Ottiene la collezione di intervalli di modifica consentita nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/alloweditranges/
---
## Worksheet.AllowEditRanges property

Ottiene la collezione di intervalli di modifica consentiti nel foglio di lavoro.

```csharp
public ProtectedRangeCollection AllowEditRanges { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAllowEditRangesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un intervallo di modifica consentita
            int index = worksheet.AllowEditRanges.Add("r1", 0, 0, 1, 1);
            ProtectedRange range = worksheet.AllowEditRanges[index];
            range.Password = "password123";

            // Proteggi il foglio di lavoro
            worksheet.Protect(ProtectionType.All);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");

            // Carica la cartella di lavoro salvata per verificare
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            ProtectedRange verifyRange = verifyWorkbook.Worksheets[0].AllowEditRanges[0];
            Console.WriteLine("Is protected with password: " + verifyRange.IsProtectedWithPassword);
        }
    }
}
```

### Vedi anche

* class [ProtectedRangeCollection](../../protectedrangecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


