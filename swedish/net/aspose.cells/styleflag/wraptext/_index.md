---
title: "StyleFlag.WrapText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag property. Inställningen för radbrytning av text kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/wraptext/
---
## StyleFlag.WrapText property

Inställningen för radbrytning av text kommer att tillämpas.

```csharp
public bool WrapText { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyWrapTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil med textbrytning aktiverad
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Skapa en stilflagga och aktivera WrapText-flaggan
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;

            // Applicera stilen på cell A1 med de angivna flaggorna
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap in the cell");
            worksheet.Cells.ApplyStyle(style, flag);

            // Auto-anpassa radhöjden för att se den radbrytna texten
            worksheet.AutoFitRow(0);

            // Spara arbetsboken
            workbook.Save("WrapTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


