---
title: "StyleFlag.StyleFlag"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-konstruktor. Skapar ett objekt med alla flaggor som falska"
type: docs
url: /sv/net/aspose.cells/styleflag/styleflag/
---
## StyleFlag constructor

Skapar ett objekt med alla flaggor satta till falskt.

```csharp
public StyleFlag()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en fet stil
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Tillämpa stil på rad 9 med StyleFlag-konstruktor
            worksheet.Cells.ApplyRowStyle(9, boldStyle, new StyleFlag { FontBold = true });

            // Sätt värde i cellen och verifiera stil
            worksheet.Cells[9, 0].PutValue("Bold Text");

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            Console.WriteLine("Style applied successfully using StyleFlag constructor.");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


