---
title: "Style.ToJson"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Methode. Konvertiere Style in JSON-Strukturdaten"
type: docs
url: /de/net/aspose.cells/style/tojson/
---
## Style.ToJson method

Konvertiere [`Style`](../) in JSON-Strukturdaten.

```csharp
public string ToJson()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodToJsonDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstelle und wende einen Stil auf Zelle B4 an
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Yellow;
            cells["B4"].SetStyle(style);

            // Konvertiere Stil in JSON
            string styleJson = style.ToJson();
            Console.WriteLine("Style JSON:");
            Console.WriteLine(styleJson);

            // Formel in Zelle B6 festlegen
            cells["B6"].Formula = "=A1";

            // Konvertiere Zelle in JSON
            string cellJson = cells["B6"].ToJson();
            Console.WriteLine("\nCell JSON:");
            Console.WriteLine(cellJson);
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


