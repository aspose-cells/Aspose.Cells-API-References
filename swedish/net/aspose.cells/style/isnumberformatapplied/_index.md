---
title: "Style.IsNumberFormatApplied"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Anger om nummerformatering ska tillämpas"
type: docs
url: /sv/net/aspose.cells/style/isnumberformatapplied/
---
## Style.IsNumberFormatApplied property

Anger om talformateringen ska tillämpas.

```csharp
public bool IsNumberFormatApplied { get; set; }
```

### Anmärkningar

Endast för namngiven stil.

### Exempel

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
            
            // Skapa en stil med talformat
            Style style = workbook.CreateStyle();
            style.Number = 14; // Format as "m/d/yyyy"
            style.IsNumberFormatApplied = true;
            
            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Verifiera att talformatet har tillämpats
            Console.WriteLine("IsNumberFormatApplied: " + style.IsNumberFormatApplied);
            Console.WriteLine("Cell value format: " + cell.GetDisplayStyle().Number);
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


