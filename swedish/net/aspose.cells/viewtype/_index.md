---
title: "Enum ViewType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ViewType enum. Representerar vyn för kalkylbladet"
type: docs
url: /sv/net/aspose.cells/viewtype/
---
## ViewType enumeration

Representerar vystyper för kalkylbladet.

```csharp
public enum ViewType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| NormalView | `0` |  |
| PageBreakPreview | `1` |  |
| PageLayoutView | `2` |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ViewTypeDemo
    {
        public static void ViewTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in vyn för kalkylbladet till PageBreakPreview
            worksheet.ViewType = ViewType.PageBreakPreview;
            
            // Spara arbetsboken
            workbook.Save("ViewTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


