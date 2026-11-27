---
title: "Style.IndentLevel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Representerar indenteringsnivån för cellen eller området. Kan endast vara ett heltal mellan 0 och 250"
type: docs
url: /sv/net/aspose.cells/style/indentlevel/
---
## Style.IndentLevel property

Representerar indenteringsnivån för cellen eller området. Kan endast vara ett heltal mellan 0 och 250.

```csharp
public int IndentLevel { get; set; }
```

### Anmärkningar

Om textens horisontella justering är inställd på ett värde annat än vänster eller höger, återställs indenteringsnivån till noll.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIndentLevelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in olika indenteringsnivåer för celler
            for (int i = 0; i < 16; i++)
            {
                Cell cell = cells[i, 0];
                Style style = cell.GetStyle();
                style.IndentLevel = i;
                style.HorizontalAlignment = TextAlignmentType.Left;
                cell.SetStyle(style);
                cell.PutValue($"Indent Level {i}");
            }

            // Spara arbetsboken
            workbook.Save("IndentLevelDemo.xlsx");
            Console.WriteLine("Workbook saved with different indent levels.");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


