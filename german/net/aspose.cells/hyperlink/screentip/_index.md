---
title: "Hyperlink.ScreenTip"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Hyperlink-Eigenschaft. Gibt den ScreenTip-Text für den angegebenen Hyperlink zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells/hyperlink/screentip/
---
## Hyperlink.ScreenTip property

Gibt den ScreenTip-Text für den angegebenen Hyperlink zurück oder legt ihn fest.

```csharp
public string ScreenTip { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyScreenTipDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Click this hyperlink:");

            // Erstellen Sie einen Hyperlink mit ScreenTip.
            int hLinkIdx = worksheet.Hyperlinks.Add("B1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks[hLinkIdx].ScreenTip = "Visit Aspose website for more information";

            // Speichere die Arbeitsmappe
            workbook.Save("HyperlinkWithScreenTip.xlsx");
        }
    }
}
```

### Siehe auch

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


