---
title: "Enum PageOrientationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PageOrientationType enum. Representerar utskriftsorienteringskonstanter"
type: docs
url: /sv/net/aspose.cells/pageorientationtype/
---
## PageOrientationType enumeration

Representerar konstanter för utskriftsorientering.

```csharp
public enum PageOrientationType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Landscape | `0` | Landskapsorientering |
| Portrait | `1` | Stående orientering |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageOrientationTypeDemo
    {
        public static void PageOrientationTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till PageSetup-objektet i kalkylbladet
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Ställ in sidans orientering till Landskap
            pageSetup.Orientation = PageOrientationType.Landscape;
            
            // Spara arbetsboken till en fil
            workbook.Save("PageOrientationTypeExample_Landscape.xlsx");

            // Ställ in sidans orientering till Stående
            pageSetup.Orientation = PageOrientationType.Portrait;
            
            // Spara arbetsboken till en annan fil
            workbook.Save("PageOrientationTypeExample_Portrait.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


