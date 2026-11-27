---
title: "Cells.StandardWidthInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar eller anger standardkolumnbredd i kalkylbladet i tum."
type: docs
url: /sv/net/aspose.cells/cells/standardwidthinch/
---
## Cells.StandardWidthInch property

Hämtar eller anger standardkolumnbredden i kalkylbladet, i enheten tum.

```csharp
public double StandardWidthInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange standardkolumnbredd i tum
            worksheet.Cells.StandardWidthInch = 1.5;

            // Ange specifik kolumnbredd i tum för demonstration
            worksheet.Cells.SetColumnWidthInch(1, 2.0);

            // Spara arbetsboken
            workbook.Save("StandardWidthInchDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


