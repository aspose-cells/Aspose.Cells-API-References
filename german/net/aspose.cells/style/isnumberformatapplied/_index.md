---
title: "Style.IsNumberFormatApplied"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt an, ob die Zahlenformatierung angewendet werden soll"
type: docs
url: /de/net/aspose.cells/style/isnumberformatapplied/
---
## Style.IsNumberFormatApplied property

Gibt an, ob die Zahlenformatierung angewendet werden soll.

```csharp
public bool IsNumberFormatApplied { get; set; }
```

### Hinweise

Nur für benannte Stile.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsNumberFormatAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie einen Stil mit Zahlenformat
            Style style = workbook.CreateStyle();
            style.Number = 14; // Format as "m/d/yyyy"
            style.IsNumberFormatApplied = true;
            
            // Wende den Stil auf eine Zelle an
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Überprüfen Sie, ob das Zahlenformat angewendet wurde
            Console.WriteLine("IsNumberFormatApplied: " + style.IsNumberFormatApplied);
            Console.WriteLine("Cell value format: " + cell.GetDisplayStyle().Number);
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


