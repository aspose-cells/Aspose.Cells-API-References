---
title: "Enum TextDirectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TextDirectionType enum. Representerar riktningen för textflödet i detta stycke"
type: docs
url: /sv/net/aspose.cells/textdirectiontype/
---
## TextDirectionType enumeration

Representerar riktningen för textflödet i detta stycke.

```csharp
public enum TextDirectionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Context | `0` |  |
| LeftToRight | `1` |  |
| RightToLeft | `2` |  |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTextDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in textriktning från höger till vänster
            Style style = cells["A1"].GetStyle();
            style.TextDirection = TextDirectionType.RightToLeft;
            cells["A1"].SetStyle(style);
            cells["A1"].PutValue("Right to Left Text");

            // Ställ in textriktning från vänster till höger
            style = cells["A2"].GetStyle();
            style.TextDirection = TextDirectionType.LeftToRight;
            cells["A2"].SetStyle(style);
            cells["A2"].PutValue("Left to Right Text");

            // Ställ in kontextuell textriktning
            style = cells["A3"].GetStyle();
            style.TextDirection = TextDirectionType.Context;
            cells["A3"].SetStyle(style);
            cells["A3"].PutValue("Context Text Direction");

            workbook.Save("TextDirectionTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


