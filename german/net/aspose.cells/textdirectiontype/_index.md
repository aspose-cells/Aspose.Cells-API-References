---
title: "Aufzählung TextDirectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TextDirectionType enum. Stellt die Richtung des Textflusses für diesen Absatz dar."
type: docs
url: /de/net/aspose.cells/textdirectiontype/
---
## TextDirectionType enumeration

Stellt die Richtung des Textflusses für diesen Absatz dar.

```csharp
public enum TextDirectionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Context | `0` |  |
| LeftToRight | `1` |  |
| RightToLeft | `2` |  |

### Beispiele

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

            // Richtung von Rechts nach Links festlegen
            Style style = cells["A1"].GetStyle();
            style.TextDirection = TextDirectionType.RightToLeft;
            cells["A1"].SetStyle(style);
            cells["A1"].PutValue("Right to Left Text");

            // Richtung von Links nach Rechts festlegen
            style = cells["A2"].GetStyle();
            style.TextDirection = TextDirectionType.LeftToRight;
            cells["A2"].SetStyle(style);
            cells["A2"].PutValue("Left to Right Text");

            // Kontext‑Text‑Richtung festlegen
            style = cells["A3"].GetStyle();
            style.TextDirection = TextDirectionType.Context;
            cells["A3"].SetStyle(style);
            cells["A3"].PutValue("Context Text Direction");

            workbook.Save("TextDirectionTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


