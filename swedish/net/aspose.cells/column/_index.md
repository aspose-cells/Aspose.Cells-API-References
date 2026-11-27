---
title: "Klass Column"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Column-klass. Representerar en enda kolumn i ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/column/
---
## Column class

Representerar en enskild kolumn i ett kalkylblad.

```csharp
public class Column
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [GroupLevel](../../aspose.cells/column/grouplevel/) { get; set; } | Hämtar gruppnivån för kolumnen. |
| [HasCustomStyle](../../aspose.cells/column/hascustomstyle/) { get; } | Indikerar om den här kolumnen har anpassade stilinställningar (annorlunda än standardinställningen som ärvs från arbetsboken). |
| [Index](../../aspose.cells/column/index/) { get; } | Hämtar indexet för den här kolumnen. |
| [IsCollapsed](../../aspose.cells/column/iscollapsed/) { get; set; } | om kolumnen är hopfälld |
| [IsHidden](../../aspose.cells/column/ishidden/) { get; set; } | Indikerar om kolumnen är dold. |
| [Style](../../aspose.cells/column/style/) { get; } | (**Obsolete.**) Hämtar stilen för den här kolumnen. |
| [Width](../../aspose.cells/column/width/) { get; set; } | Hämtar och anger kolumnbredden i tecken. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ApplyStyle](../../aspose.cells/column/applystyle/)(Style, StyleFlag) | Tillämpar format för en hel kolumn. |
| [GetStyle](../../aspose.cells/column/getstyle/)() | Hämtar stilen för den här kolumnen. |
| [SetStyle](../../aspose.cells/column/setstyle/)(Style) | Anger stilen för den här kolumnen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnDemo
    {
        public static void ColumnExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Hämtning av referensen till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ny stil i arbetsboken
            Style style = workbook.CreateStyle();

            // Ställer in bakgrundsfärgen till blå
            style.BackgroundColor = Color.Blue;

            // Ställer in förgrundsfärgen till röd
            style.ForegroundColor = Color.Red;

            // Ställer in bakgrundsmönster
            style.Pattern = BackgroundType.DiagonalStripe;

            // Ny stilflagga
            StyleFlag styleFlag = new StyleFlag();

            // Ställ in alla stilar
            styleFlag.All = true;

            // Hämta första kolumnen
            Column column = worksheet.Cells.Columns[0];

            // Applicera stil på första kolumnen
            column.ApplyStyle(style, styleFlag);

            // Ställer in ytterligare egenskaper
            column.Width = 20.0; // Setting the column width
            column.IsHidden = false; // Setting the column visibility
            column.IsCollapsed = false; // Setting the column collapsed state

            // Sparar Excel-filen
            workbook.Save("ColumnExample.xlsx");
            workbook.Save("ColumnExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


