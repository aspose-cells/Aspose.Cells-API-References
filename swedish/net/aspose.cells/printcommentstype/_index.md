---
title: "Enum PrintCommentsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PrintCommentsType enum. Representerar hur kommentarer skrivs ut med bladet"
type: docs
url: /sv/net/aspose.cells/printcommentstype/
---
## PrintCommentsType enumeration

Representerar hur kommentarer skrivs ut med bladet.

```csharp
public enum PrintCommentsType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| PrintInPlace | `0` | Representerar att skriva ut kommentarer som de visas på bladet. |
| PrintNoComments | `1` | Representerar att inte skriva ut kommentarer. |
| PrintSheetEnd | `2` | Representerar att skriva ut kommentarer i slutet av bladet. |
| PrintWithThreadedComments | `3` | Representerar att skriva ut kommentarer som de visas på bladet, inklusive trådade kommentarer. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintCommentsTypeDemo
    {
        public static void PrintCommentsTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till några kommentarer i arbetsbladet
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment.";

            commentIndex = worksheet.Comments.Add("B2");
            comment = worksheet.Comments[commentIndex];
            comment.Note = "This is another comment.";

            // Ställ in utskriftskommentarstypen i sidinställningarna
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;

            // Spara arbetsboken till en fil
            workbook.Save("PrintCommentsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully with comments printed at the end of the sheet.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


