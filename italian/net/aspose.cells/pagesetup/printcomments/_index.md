---
title: "PageSetup.PrintComments"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PageSetup proprietà. Rappresenta il modo in cui i commenti vengono stampati con il foglio"
type: docs
url: /it/net/aspose.cells/pagesetup/printcomments/
---
## PageSetup.PrintComments property

Rappresenta il modo in cui i commenti vengono stampati con il foglio.

```csharp
public PrintCommentsType PrintComments { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCommentsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = sheet.Comments.Add("A1");
            Comment comment = sheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Imposta diverse opzioni di stampa dei commenti e dimostra i loro effetti
            sheet.PageSetup.PrintComments = PrintCommentsType.PrintInPlace;
            Console.WriteLine("PrintComments set to PrintInPlace");

            sheet.PageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;
            Console.WriteLine("PrintComments set to PrintSheetEnd");

            sheet.PageSetup.PrintComments = PrintCommentsType.PrintNoComments;
            Console.WriteLine("PrintComments set to PrintNoComments");

            // Salva la cartella di lavoro per dimostrare che le impostazioni persistono
            workbook.Save("PrintCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* enum [PrintCommentsType](../../printcommentstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


