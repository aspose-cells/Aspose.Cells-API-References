---
title: "StyleFlag.Indent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag property. Indent-nivåinställning kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/indent/
---
## StyleFlag.Indent property

Inställning för indenteringsnivå kommer att tillämpas.

```csharp
public bool Indent { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyIndentDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil med indenteringsnivå
            Style style = workbook.CreateStyle();
            style.IndentLevel = 2;
            style.HorizontalAlignment = TextAlignmentType.Left;

            // Skapa stilflagga med Indent-egenskapen satt
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Indent = true;

            // Applicera data till celler
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                }
            }

            // Applicera stilen med indentering på ett intervall
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 5, 5);
            range.ApplyStyle(style, styleFlag);

            // Verifiera att stilen har tillämpats
            Cell cell = worksheet.Cells["A1"];
            Style appliedStyle = cell.GetStyle();
            Console.WriteLine($"Indent Level: {appliedStyle.IndentLevel}");
            Console.WriteLine($"Alignment: {appliedStyle.HorizontalAlignment}");

            // Spara arbetsboken
            workbook.Save("IndentStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


