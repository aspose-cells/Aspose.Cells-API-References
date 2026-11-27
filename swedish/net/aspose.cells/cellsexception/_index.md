---
title: "Klass CellsException"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellsException-klass. Undantaget som kastas när ett specificerat fel i Aspose.Cells inträffar"
type: docs
url: /sv/net/aspose.cells/cellsexception/
---
## CellsException class

Undantaget som kastas när ett specificerat fel i Aspose.Cells inträffar.

```csharp
public class CellsException : ApplicationException
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Code](../../aspose.cells/cellsexception/code/) { get; } | Representerar anpassad undantagskod. |

### Exempel

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
                // Simulera en operation som orsakar ett undantag
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                // Avsiktligt orsaka ett undantag genom att komma åt en ogiltig cell
                Cell cell = worksheet.Cells["InvalidCellAddress"];
            }
            catch (CellsException ex)
            {
                // Hantera CellsException
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


