---
title: "Style.IsFillApplied"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt an, ob die Füllformatierung angewendet werden soll."
type: docs
url: /de/net/aspose.cells/style/isfillapplied/
---
## Style.IsFillApplied property

Gibt an, ob die Füllformatierung angewendet werden soll.

```csharp
public bool IsFillApplied { get; set; }
```

### Hinweise

Nur für benannte Stile.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFillAppliedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie einen Stil
            Style style = workbook.CreateStyle();
            
            // Anfangs sollte IsFillApplied false sein.
            Console.WriteLine("IsFillApplied (initial): " + style.IsFillApplied);
            
            // Wenden Sie Füll-Einstellungen an.
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Nach dem Festlegen der Füll-Eigenschaften sollte IsFillApplied true sein
            Console.WriteLine("IsFillApplied (after setting fill): " + style.IsFillApplied);
            
            // Wende den Stil auf eine Zelle an
            worksheet.Cells["A1"].SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("IsFillAppliedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


