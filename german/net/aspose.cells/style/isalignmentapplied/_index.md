---
title: "Style.IsAlignmentApplied"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt an, ob die Ausrichtungsformatierung angewendet werden soll"
type: docs
url: /de/net/aspose.cells/style/isalignmentapplied/
---
## Style.IsAlignmentApplied property

Gibt an, ob die Ausrichtungsformatierung angewendet werden soll.

```csharp
public bool IsAlignmentApplied { get; set; }
```

### Hinweise

Nur für benannte Stile.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsAlignmentAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            
            // Ausrichtungseigenschaften festlegen
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            
            // Anwendung der Ausrichtung aktivieren
            style.IsAlignmentApplied = true;
            
            cell.SetStyle(style);
            
            // Überprüfen Sie, ob die Ausrichtung angewendet wurde
            Console.WriteLine("Alignment applied: " + style.IsAlignmentApplied);
            Console.WriteLine("Horizontal Alignment: " + style.HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + style.VerticalAlignment);
            
            workbook.Save("AlignmentExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


