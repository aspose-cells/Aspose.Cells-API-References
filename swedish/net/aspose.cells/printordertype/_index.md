---
title: "Enum PrintOrderType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PrintOrderType enum. Representerar utskriftsordningskonstanter"
type: docs
url: /sv/net/aspose.cells/printordertype/
---
## PrintOrderType enumeration

Representerar konstanter för utskriftsordning.

```csharp
public enum PrintOrderType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| DownThenOver | `0` | Ned, sedan över |
| OverThenDown | `1` | Över, sedan ned |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintOrderTypeDemo
    {
        public static void PrintOrderTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt PageSetup-objektet
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in utskriftsordning till DownThenOver
            pageSetup.Order = PrintOrderType.DownThenOver;

            // Ställ in några andra sidinställningsegenskaper för demonstration
            pageSetup.PrintArea = "A1:D10";
            pageSetup.PrintTitleRows = "$1:$1";
            pageSetup.PrintTitleColumns = "$A:$A";
            pageSetup.CenterHorizontally = true;
            pageSetup.CenterVertically = true;

            // Spara arbetsboken
            workbook.Save("PrintOrderTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


