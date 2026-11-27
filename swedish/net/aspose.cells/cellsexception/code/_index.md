---
title: "CellsException.Code"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsException-egenskap. Representerar anpassad undantagskod"
type: docs
url: /sv/net/aspose.cells/cellsexception/code/
---
## CellsException.Code property

Representerar anpassad undantagskod.

```csharp
public ExceptionType Code { get; }
```

### Exempel

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
                // Skapa en arbetsbok och försök att komma åt ett icke-existerande kalkylblad
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets["NonExistentSheet"];
            }
            catch (CellsException e)
            {
                // Demonstrera användning av Code-egenskapen
                Console.WriteLine($"Error Code: {e.Code}");
                Console.WriteLine($"Error Message: {e.Message}");
            }
        }
    }
}
```

### Se även

* enum [ExceptionType](../../exceptiontype/)
* class [CellsException](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


