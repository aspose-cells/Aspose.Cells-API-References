---
title: "Klasse CellsException"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellsException Klasse. Die Ausnahme, die ausgelöst wird, wenn ein von Aspose.Cells spezifizierter Fehler auftritt"
type: docs
url: /de/net/aspose.cells/cellsexception/
---
## CellsException class

Die Ausnahme, die ausgelöst wird, wenn ein von Aspose.Cells spezifizierter Fehler auftritt.

```csharp
public class CellsException : ApplicationException
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Code](../../aspose.cells/cellsexception/code/) { get; } | Stellt benutzerdefinierten Ausnahmecode dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;
    using System.Collections;

    public class CellsExceptionDemo
    {
        public static void CellsExceptionExample()
        {
            try
            {
                // Simuliere eine Operation, die eine Ausnahme verursacht
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                // Absichtlich eine Ausnahme auslösen, indem auf eine ungültige Zelle zugegriffen wird
                Cell cell = worksheet.Cells["InvalidCellAddress"];
            }
            catch (CellsException ex)
            {
                // Behandle die CellsException
                Console.WriteLine("Aspose.Cells.CellsException caught!");
                Console.WriteLine($"Code: {ex.Code}");
                Console.WriteLine($"Message: {ex.Message}");
                Console.WriteLine($"TargetSite: {ex.TargetSite}");
                Console.WriteLine($"StackTrace: {ex.StackTrace}");
                Console.WriteLine($"HelpLink: {ex.HelpLink}");
                Console.WriteLine($"Source: {ex.Source}");
                Console.WriteLine($"HResult: {ex.HResult}");
                if (ex.InnerException != null)
                {
                    Console.WriteLine($"InnerException: {ex.InnerException.Message}");
                }
                foreach (DictionaryEntry entry in ex.Data)
                {
                    Console.WriteLine($"Data: {entry.Key} = {entry.Value}");
                }
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


