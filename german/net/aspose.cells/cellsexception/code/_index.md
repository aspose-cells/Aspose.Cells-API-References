---
title: "CellsException.Code"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsException-Eigenschaft. Stellt benutzerdefinierten Ausnahmecode dar"
type: docs
url: /de/net/aspose.cells/cellsexception/code/
---
## CellsException.Code property

Stellt benutzerdefinierten Ausnahmecode dar.

```csharp
public ExceptionType Code { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsExceptionPropertyCodeDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine Arbeitsmappe und versuche, auf ein nicht vorhandenes Arbeitsblatt zuzugreifen
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets["NonExistentSheet"];
            }
            catch (CellsException e)
            {
                // Verwendung der Code-Eigenschaft demonstrieren
                Console.WriteLine($"Error Code: {e.Code}");
                Console.WriteLine($"Error Message: {e.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [ExceptionType](../../exceptiontype/)
* class [CellsException](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


