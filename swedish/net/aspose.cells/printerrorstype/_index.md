---
title: "Enum PrintErrorsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PrintErrorsType enum. Representerar konstanter för utskriftsfel"
type: docs
url: /sv/net/aspose.cells/printerrorstype/
---
## PrintErrorsType enumeration

Representerar konstanter för utskriftsfel.

```csharp
public enum PrintErrorsType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| PrintErrorsBlank | `0` | Representerar att fel inte ska skrivas ut. |
| PrintErrorsDash | `1` | Representerar att skriva ut fel som "--". |
| PrintErrorsDisplayed | `2` | Representerar att skriva ut fel som visas. |
| PrintErrorsNA | `3` | Representerar att skriva ut fel som "#N/A". |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintErrorsTypeDemo
    {
        public static void PrintErrorsTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till PageSetup för kalkylbladet
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in olika typer av utskriftsfel
            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            workbook.Save("PrintErrorsBlank.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            workbook.Save("PrintErrorsDash.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDisplayed;
            workbook.Save("PrintErrorsDisplayed.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsNA;
            workbook.Save("PrintErrorsNA.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


