---
title: "Style.TextDirection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Stellt die Lesereihenfolge des Textes dar"
type: docs
url: /de/net/aspose.cells/style/textdirection/
---
## Style.TextDirection property

Stellt die Lesereihenfolge des Textes dar.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyTextDirectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setze verschiedene Textausrichtungen
            Style style1 = cells["A1"].GetStyle();
            style1.TextDirection = TextDirectionType.Context;
            cells["A1"].SetStyle(style1);
            cells["A1"].PutValue("Context Direction");

            Style style2 = cells["A2"].GetStyle();
            style2.TextDirection = TextDirectionType.LeftToRight;
            cells["A2"].SetStyle(style2);
            cells["A2"].PutValue("LeftToRight Direction");

            Style style3 = cells["A3"].GetStyle();
            style3.TextDirection = TextDirectionType.RightToLeft;
            cells["A3"].SetStyle(style3);
            cells["A3"].PutValue("RightToLeft Direction");

            // Speichere die Arbeitsmappe
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextDirectionType](../../textdirectiontype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


