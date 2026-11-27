---
title: "PageSetup.PrintComments"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskapen. Representerar hur kommentarer skrivs ut med bladet"
type: docs
url: /sv/net/aspose.cells/pagesetup/printcomments/
---
## PageSetup.PrintComments property

Representerar hur kommentarer skrivs ut med bladet.

```csharp
public PrintCommentsType PrintComments { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCommentsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = sheet.Comments.Add("A1");
            Comment comment = sheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Ställ in olika utskriftskommentaralternativ och demonstrera deras effekter
            sheet.PageSetup.PrintComments = PrintCommentsType.PrintInPlace;
            Console.WriteLine("PrintComments set to PrintInPlace");

            sheet.PageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;
            Console.WriteLine("PrintComments set to PrintSheetEnd");

            sheet.PageSetup.PrintComments = PrintCommentsType.PrintNoComments;
            Console.WriteLine("PrintComments set to PrintNoComments");

            // Spara arbetsboken för att demonstrera att inställningarna kvarstår
            workbook.Save("PrintCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [PrintCommentsType](../../printcommentstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


