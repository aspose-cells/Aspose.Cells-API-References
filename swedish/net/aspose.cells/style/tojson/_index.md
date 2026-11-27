---
title: "Style.ToJson"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-metod. Konvertera Style till JSON-strukturdatan"
type: docs
url: /sv/net/aspose.cells/style/tojson/
---
## Style.ToJson method

Konvertera [`Style`](../) till JSON-strukturdatan.

```csharp
public string ToJson()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodToJsonDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa och applicera en stil på cell B4
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Yellow;
            cells["B4"].SetStyle(style);

            // Konvertera stil till JSON
            string styleJson = style.ToJson();
            Console.WriteLine("Style JSON:");
            Console.WriteLine(styleJson);

            // Ange formel i cell B6
            cells["B6"].Formula = "=A1";

            // Konvertera cell till JSON
            string cellJson = cells["B6"].ToJson();
            Console.WriteLine("\nCell JSON:");
            Console.WriteLine(cellJson);
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


