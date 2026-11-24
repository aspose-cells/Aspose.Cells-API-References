---
title: "Comment.HeightCM"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Gibt die Höhe des Kommentars in Zentimetern an"
type: docs
url: /de/net/aspose.cells/comment/heightcm/
---
## Comment.HeightCM property

Stellt die Höhe des Kommentars in Zentimetern dar.

```csharp
public double HeightCM { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightCMDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Setze Kommentartext
            comment.Note = "Sample comment";
            
            // Setzen Sie die Kommentarhöhe in Zentimetern
            comment.HeightCM = 1.5;
            
            // Speichere die Arbeitsmappe
            workbook.Save("CommentHeightCMDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


