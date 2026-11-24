---
title: "Enum PrintCommentsType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PrintCommentsType enum. Gibt an, wie Kommentare mit dem Blatt gedruckt werden"
type: docs
url: /de/net/aspose.cells/printcommentstype/
---
## PrintCommentsType enumeration

Stellt die Art und Weise dar, wie Kommentare mit dem Blatt gedruckt werden.

```csharp
public enum PrintCommentsType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| PrintInPlace | `0` | Stellt dar, Kommentare wie im Blatt angezeigt zu drucken. |
| PrintNoComments | `1` | Stellt dar, Kommentare nicht zu drucken. |
| PrintSheetEnd | `2` | Stellt dar, Kommentare am Ende des Blattes zu drucken. |
| PrintWithThreadedComments | `3` | Stellt dar, Kommentare wie im Blatt angezeigt zu drucken, einschließlich Threaded-Kommentaren. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintCommentsTypeDemo
    {
        public static void PrintCommentsTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Kommentare zum Arbeitsblatt hinzu
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment.";

            commentIndex = worksheet.Comments.Add("B2");
            comment = worksheet.Comments[commentIndex];
            comment.Note = "This is another comment.";

            // Legen Sie den Druckkommentar‑Typ in den Seiteneinstellungen fest
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;

            // Speichere die Arbeitsmappe in einer Datei
            workbook.Save("PrintCommentsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully with comments printed at the end of the sheet.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


