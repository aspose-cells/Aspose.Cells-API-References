---
title: "StyleFlag.All"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Alla egenskaper kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/all/
---
## StyleFlag.All property

Alla egenskaper kommer att tillämpas.

```csharp
public bool All { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyAllDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa en stil med solid röd bakgrund
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;

            // Skapa en stilflagga med All-egenskapen satt till true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.All = true;

            // Tillämpa stilen på den första kolumnen
            Column column = cells.Columns[0];
            column.ApplyStyle(style, styleFlag);

            // Verifiera att stilen har tillämpats på cellerna i kolumnen
            Cell cell = cells[0, 0];
            Style appliedStyle = cell.GetStyle();
            
            Console.WriteLine("Pattern: " + appliedStyle.Pattern);
            Console.WriteLine("Color: " + appliedStyle.ForegroundColor);
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


