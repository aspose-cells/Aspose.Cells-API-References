---
title: "Spinner.Max"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Spinner-egenskap. Hämtar eller anger det maximala värdet för en rullningslist eller spinnerintervall"
type: docs
url: /sv/net/aspose.cells.drawing/spinner/max/
---
## Spinner.Max property

Hämtar eller anger det maximala värdet för ett rullningslist‑ eller spinnerintervall.

```csharp
public int Max { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMaxDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Spinner spinner = sheet.Shapes.AddSpinner(1, 1, 0, 0, 100, 100);
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;

            Console.WriteLine($"Spinner Max Value: {spinner.Max}");
        }
    }
}
```

### Se även

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


