---
title: "Worksheet.ErrorCheckOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt die Fehlerprüfungs-Einstellung zurück, die auf bestimmte Bereiche angewendet wird"
type: docs
url: /de/net/aspose.cells/worksheet/errorcheckoptions/
---
## Worksheet.ErrorCheckOptions property

Liest die Fehlerprüfungs-Einstellung, die auf bestimmte Bereiche angewendet wird.

```csharp
public ErrorCheckOptionCollection ErrorCheckOptions { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyErrorCheckOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fehlerprüfungsoptionen aktivieren
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            ErrorCheckOption option = options[0]; // Properly access first option using indexer
            option.SetErrorCheck(ErrorCheckType.TextDate, true);
            option.AddRange(CellArea.CreateCellArea(0, 0, 10, 10));
            
            // Anzahl der Bereiche für die Option ermitteln
            int rangeCount = option.GetCountOfRange();
            Console.WriteLine("Number of ranges in ErrorCheckOption: " + rangeCount);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ErrorCheckOptionsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ErrorCheckOptionCollection](../../errorcheckoptioncollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


