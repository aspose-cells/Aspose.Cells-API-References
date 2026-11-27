---
title: "Comment.AutoSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment property. Anger om storleken på kommentaren justeras automatiskt enligt dess innehåll. Obs! I vissa speciella fall, såsom Mac-miljö, kan den här inställningen inte träda i kraft. Om den här inställningen inte har någon effekt, ersätt den med FitToTextSize"
type: docs
url: /sv/net/aspose.cells/comment/autosize/
---
## Comment.AutoSize property

Anger om kommentarsstorleken justeras automatiskt enligt dess innehåll. Obs: I vissa speciella fall (t.ex. Mac-miljö) kan denna inställning vara utan effekt. Om den inte har någon effekt, ersätt den med FitToTextSize().

```csharp
public bool AutoSize { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment that will auto-size to fit its content.";

            // Ställ in AutoSize till true
            comment.AutoSize = true;

            // Spara arbetsboken
            workbook.Save("CommentAutoSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


