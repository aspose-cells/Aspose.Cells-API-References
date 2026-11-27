---
title: "Range.IsBlank"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Anger om området innehåller värden"
type: docs
url: /sv/net/aspose.cells/range/isblank/
---
## Range.IsBlank method

Anger om området innehåller värden.

```csharp
public bool IsBlank()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa ett område och kontrollera om det är tomt (ska vara true)
            Aspose.Cells.Range range1 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank: " + range1.IsBlank());

            // Sätt ett värde i en cell och kontrollera igen (ska vara false)
            cells["B2"].PutValue("Test");
            Aspose.Cells.Range range2 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank after adding value: " + range2.IsBlank());
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


