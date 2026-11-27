---
title: "Style.IsAlignmentApplied"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Anger om justeringsformatering ska tillämpas"
type: docs
url: /sv/net/aspose.cells/style/isalignmentapplied/
---
## Style.IsAlignmentApplied property

Anger om justeringsformateringen ska tillämpas.

```csharp
public bool IsAlignmentApplied { get; set; }
```

### Anmärkningar

Endast för namngiven stil.

### Exempel

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
            
            // Ställ in justeringsegenskaper
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            
            // Aktivera tillämpning av justering
            style.IsAlignmentApplied = true;
            
            cell.SetStyle(style);
            
            // Verifiera att justering har tillämpats
            Console.WriteLine("Alignment applied: " + style.IsAlignmentApplied);
            Console.WriteLine("Horizontal Alignment: " + style.HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + style.VerticalAlignment);
            
            workbook.Save("AlignmentExample.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


