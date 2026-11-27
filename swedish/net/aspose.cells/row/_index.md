---
title: "Klass Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Row class. Representerar en enskild rad i ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/row/
---
## Row class

Representerar en enskild rad i ett kalkylblad.

```csharp
public class Row : IEnumerable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FirstCell](../../aspose.cells/row/firstcell/) { get; } | Hämtar det första cellobjektet i raden. |
| [FirstDataCell](../../aspose.cells/row/firstdatacell/) { get; } | Hämtar den första icke‑tomma cellen i raden. |
| [GroupLevel](../../aspose.cells/row/grouplevel/) { get; set; } | Hämtar gruppnivån för raden. |
| [HasCustomStyle](../../aspose.cells/row/hascustomstyle/) { get; } | Anger om den här raden har anpassade stilinställningar(skiljer sig från standardinställningen som ärvs från arbetsboken). |
| [Height](../../aspose.cells/row/height/) { get; set; } | Hämtar och anger radens höjd i enheten punkter. |
| [Index](../../aspose.cells/row/index/) { get; } | Hämtar indexet för den här raden. |
| [IsBlank](../../aspose.cells/row/isblank/) { get; } | Anger om raden innehåller någon data |
| [IsCollapsed](../../aspose.cells/row/iscollapsed/) { get; set; } | om raden är hopfälld |
| [IsHeightMatched](../../aspose.cells/row/isheightmatched/) { get; set; } | Anger om radens höjd matchar den aktuella standardteckensnittinställningen i arbetsboken. Sant för den här egenskapen betyder också att radens höjd är "automatisk" utan att ett anpassat höjdvärde har satts av användaren. |
| [IsHidden](../../aspose.cells/row/ishidden/) { get; set; } | Anger om raden är dold. |
| [Item](../../aspose.cells/row/item/) { get; } | Hämtar cellen. |
| [LastCell](../../aspose.cells/row/lastcell/) { get; } | Hämtar det sista cellobjektet i raden. |
| [LastDataCell](../../aspose.cells/row/lastdatacell/) { get; } | Hämtar den sista icke‑tomma cellen i raden. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ApplyStyle](../../aspose.cells/row/applystyle/)(Style, StyleFlag) | Tillämpar format för en hel rad. |
| [CopySettings](../../aspose.cells/row/copysettings/)(Row, bool) | Kopierar radinställningar, såsom stil, höjd, synlighet, ...etc. |
| override [Equals](../../aspose.cells/row/equals/#equals_1)(object) | Kontrollerar om detta objekt refererar till samma rad som ett annat. |
| [Equals](../../aspose.cells/row/equals/#equals)(Row) | Kontrollerar om detta objekt refererar till samma rad som ett annat radobjekt. |
| [GetCellByIndex](../../aspose.cells/row/getcellbyindex/)(int) | Hämta cellen med ett specifikt index i cellsamlingen för den här raden. |
| [GetCellOrNull](../../aspose.cells/row/getcellornull/)(int) | Hämtar cellen eller null på det specifika indexet. |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator)() | Hämtar cellernas enumerator |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator_1)(bool, bool) | Hämtar en enumerator som itererar celler genom den här raden. |
| [GetStyle](../../aspose.cells/row/getstyle/)() | Hämtar stilen för den här raden. |
| [SetStyle](../../aspose.cells/row/setstyle/)(Style) | Anger stilen för den här raden. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;
    using System.Collections;

    public class RowDemo
    {
        public static void RowExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Hämtning av referensen till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett stilobjekt
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

            // Hämta första raden
            Row row = worksheet.Cells.Rows[0];

            // Applicera stil på första raden
            row.ApplyStyle(style, styleFlag);

            // Inställning av radens egenskaper
            row.Height = 20.0;
            row.IsHidden = false;
            row.IsCollapsed = false;
            row.GroupLevel = 1;
            row.IsHeightMatched = true;

            // Åtkomst till celler i raden
            Cell firstCell = row.FirstCell;
            Cell firstDataCell = row.FirstDataCell;
            Cell lastCell = row.LastCell;
            Cell lastDataCell = row.LastDataCell;

            // Kontrollerar om raden är tom
            bool isBlank = row.IsBlank;

            // Kontrollerar om raden har anpassad stil
            bool hasCustomStyle = row.HasCustomStyle;

            // Hämtar radens index
            int rowIndex = row.Index;

            // Hämtar en cell efter index
            Cell cellByIndex = row.GetCellByIndex(0);

            // Hämtar radens stil
            Style rowStyle = row.GetStyle();

            // Ställer in radens stil
            row.SetStyle(rowStyle);

            // Kopierar inställningar från en annan rad
            Row sourceRow = worksheet.Cells.Rows[1];
            row.CopySettings(sourceRow, true);

            // Enumererar celler i raden
            IEnumerator cellEnumerator = row.GetEnumerator();
            while (cellEnumerator.MoveNext())
            {
                Cell cell = (Cell)cellEnumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Sparar Excel-filen
            workbook.Save("RowExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


