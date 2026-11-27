---
title: "Comment.HeightCM"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment-egenskap. Representerar kommentaren höjd i enheten centimeter"
type: docs
url: /sv/net/aspose.cells/comment/heightcm/
---
## Comment.HeightCM property

Representerar kommentarsens höjd i centimeter.

```csharp
public double HeightCM { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightCMDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Ställ in kommentartext
            comment.Note = "Sample comment";
            
            // Ställ in kommentaren höjd i centimeter
            comment.HeightCM = 1.5;
            
            // Spara arbetsboken
            workbook.Save("CommentHeightCMDemo.xlsx");
        }
    }
}
```

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


